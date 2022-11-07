<!-- eslint-disable prettier/prettier -->
<template>
  <div> 
    <form>
        <label>Input email here:</label>
        <input type="email" required v-model="email"/>
        <label >Enter password:</label>
        <input type="password" v-model="password">
        <label>Role</label>
        <select v-model="role" >
            <option value="developer">Web developer</option>
            <option value="desiner">Designer</option>
            <option value="mentor">Mentor</option>
        </select>
        <div class="terms">
            <input type="checkbox" required v-model="accept"/>
            <label>Accept all terms</label>
        </div>
    </form>
    <div>
        <p>Email: {{email}}</p>
        <p>Password: {{password}}</p>
        <p>Role: {{role}}</p>
        <p>Accepting terms: {{accept}}</p>
    </div>
  </div>
</template> 
<script>
export default {
  data() {
    return {
      email: "",
      password: "",
      role: "",
      accept: false,
    };
  },
};
</script>
<style>
form {
  max-width: 420px;
  margin: 30px auto;
  background: white;
  text-align: left;
  padding: 40px;
  border-radius: 10px;
  color: #aaaa;
  display: inline-block;
}
label {
  color: #aaaa;
  display: inline-block;
  margin: 25px 0 15px;
  font-size: 0.6em;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-weight: bold;
}
input,
select {
  display: block;
  padding: 10px 6px;
  width: 100%;
  box-sizing: border-box;
  border: none;
  border-bottom: 1px solid #ddd;
  color: #555;
}
input[type="chekbox"] {
  display: inline-block;
  width: 16px;
  margin: 0 10px 0 0;
  position: relative;
  top: 2px;
}
.terms {
  display: flex;
  flex-wrap: nowrap;
}
</style>

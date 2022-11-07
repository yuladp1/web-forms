<!-- eslint-disable prettier/prettier -->
<template>
  <div> 
    <form>
        <label>Input email here:</label>
      <input type="email" required />
    </form>
  </div>
</template> 
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
input {
  display: block;
  padding: 10px 6px;
  width: 100%;
  box-sizing: border-box;
  border: none;
}
</style>

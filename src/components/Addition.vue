<template>

<div id="app">
<div class="row">
    <input v-model.number="num1" type="number" />  <span>+</span>
    <input v-model.number="num2" type="number" />  <span>=</span>
    <span>{{ num1+num2 }}</span>
</div>
  <div class="list">
    <select v-model="name">
      <option>Carne Asada</option>
      <option>Pollo</option> 
      <option>Bean</option>
      <option>Al Pastor</option>
    </select>
    <p v-if="name">My favorite kind of taco is {{ name }}</p>        
  </div> 
</div> 

</template>

<script>
    export default {
    name:'addition',
     data() {
            return {
            num1: 0,
            num2: 0,
            name: ''
            }
        }
}
</script>

<style>
.row {
  margin: 40px;
  display: flex;
  justify-content: center;
  font-family: 'Work Sans', sans-serif;
}

input, span {
  padding: 15px;
  font-size: 25px;
  font-family: 'Work Sans', sans-serif;
}

input {
  width: 100px;
}

span {
  width: 10px;
}
</style>
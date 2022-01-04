<template>
  <div id="app">
    <h1>Calculadora</h1>
    <calculator />
  </div>
</template>

<script>
import Calculator from '@/views/Calculator.vue'

export default {
  name: 'App',
  components: {
    Calculator
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  background: #4ca1af; 
  background: -webkit-linear-gradient(to right, #4ca1af, #c4e0e5); 
  background: linear-gradient(to right, #4ca1af, #c4e0e5); 
}

* {
  margin: 0;
  padding: 0;
}

</style>

<template>
  <div id="app">
  <h1>ToUppercaseConverter</h1>
  
  <input  v-model="message" placeholder="Enter a string"  @input="v => { message = v.toUpperCase()}"> <br>
  <p>output :{{message.toUpperCase()}}</p>


    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
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
  margin-top: 60px;
}
</style>

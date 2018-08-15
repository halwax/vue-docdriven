<template>
  <div id="app">
    <div id="app-header">
      <i class="fa fa-file-text fa-3x"> DocDriven</i>
    </div>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import 'font-awesome/css/font-awesome.css'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app-header {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 30px;
}
</style>

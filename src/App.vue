<template>
  <div id="app">
    <div id="app-header">
      <i class="fa fa-file-text fa-3x"> DocDriven</i>
    </div>
    <ascii-doctor :ascii-doc-text="asciiDocText"></ascii-doctor>
  </div>
</template>

<script>
import AsciiDoctor from './components/AsciiDoctor.vue'
import 'font-awesome/css/font-awesome.css'

export default {
  name: 'app',
  components: {
    AsciiDoctor
  },
  data() {
    return {
      asciiDocText : `
= Hello, DocDriven!

An introduction to http://docdriven.org[DocDriven].

== Features

* AsciiDoctor
`
    }
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

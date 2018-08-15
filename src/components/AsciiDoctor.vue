<template>
  <div class="app-asciidoctor" v-html="asciiDocHtml"></div>
</template>

<script>
import Asciidoctor from 'asciidoctor.js';

export default {
  name: 'AsciiDoctor',
  props: {
    asciiDocText: String
  },
  data() {
    var asciidoctor = Asciidoctor(); 
    var asciiDocHtml = asciidoctor.convert(this.asciiDocText); 
    return {
      asciiDocHtml : asciiDocHtml
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.app-asciidoctor {
    margin: auto;
    width: 50%;
    padding: 10px;
}
</style>

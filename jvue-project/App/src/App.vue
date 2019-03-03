<template>
  <div id="app" class="container center">
    <img src="./assets/logo.png">
    
    <ul class="nospace section-padding">
      <li>Author: {{ author }}</li>
      <li>Date: {{ date }}</li>
      <li>Site: <a href="https://jonathanslima.github.io" target="_blank">jonathanslima.github.io</a></li>
    </ul>

    <presentation :author="author" :txtpresentation="txtpresentation"></presentation>
  </div>
</template>

<script>
import Presentation from './components/Presentation.vue'

let date = new Date();

export default {
  components: {
    'presentation': Presentation
  },
  name: 'app',
  data () {
    return {
      author: 'jonathanslima',
      date: date.toLocaleDateString('pt-br'),
      txtpresentation: 'Theme based in Webpack Simple'
    }
  }
}
</script>

<style lang="scss">
  @import './src/assets/sass/main.scss'
</style>

<template>
  <div id="app">
    <iframe width="100%" height="500" scrolling="no"
    :src="`${baseUrl}web/viewer.html?file=${baseUrl}web/compressed.tracemonkey-pldi-09.pdf`"></iframe>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  },
  data () {
    return {
      baseUrl: process.env.BASE_URL
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

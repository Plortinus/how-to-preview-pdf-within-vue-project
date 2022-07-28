# how-to-preview-pdf-within-vue-project

如何在Vue项目中使用pdf.js进行pdf预览代码

```html
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
```

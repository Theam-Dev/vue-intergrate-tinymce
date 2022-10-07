<template>
  <div id="app">
    <tinymce id="d1" v-model="data"></tinymce>
    <button type="button" @click="clickHandler">Reset</button>
    <div>{{ data }}</div>
  </div>
</template>
<script>
import tinymce from './components/HelloWorld.vue'
export default {
  name: 'app',
  components: {
    tinymce
  },
  data(){
      return {
          data : '<p>Hello from tinymce</p>'
      };
  },
  methods: {
      clickHandler(){
          this.data = 'You reseted tinymce\'s content';
      }
  }
}
</script>
<style>
#app {
  padding: 10px;
}
</style>

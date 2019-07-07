<template>
  <div id="app">
      <HelloWorld/>
      <a-input/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>

<style>
  @import './assets/css/style.css';
</style>

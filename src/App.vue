<template>
  <DLogin/>
</template>

<script>

// import HelloWorld from './components/HelloWorld.vue'
// import DLogin from './components/Input/Input.vue'
import DLogin from './app/Login/Login.vue'

export default {
  name: 'app',
  components: {
    DLogin,
    // DHeader,
    // HelloWorld
  }
}
</script>

<style>
  @import './assets/css/style.css';
</style>

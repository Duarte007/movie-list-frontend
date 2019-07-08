<template>
  <div class="header">
      <div class="login">
        <DInput inputStyle="d-input"/>
        <DInput/>
        <a-button type="primary">Entrar</a-button>
      </div>
  </div>
</template>

<script>

// import HelloWorld from './components/HelloWorld.vue'
import DInput from './components/Input/Input.vue'
// import DHeader from './components/Header/Header.vue'

export default {
  name: 'app',
  components: {
    DInput,
    // DHeader,
    // HelloWorld
  }
}
</script>

<style>
  @import './assets/css/style.css';
</style>

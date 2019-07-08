<template>
    <div>
        <label for="a">Teste</label>
        <input :class="inputStyle ? inputStyle : 'd-input'" name="a"/>
    </div>
</template>

<script>
export default {
  name: 'Input',
  props: {
    inputStyle: String
  }
}
</script>

<style>
    @import './Input.css';
</style>

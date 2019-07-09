<template>
    <div :class="classDiv">
        <label>{{label ? label : ''}}<br>
          <input class="d-input" :class="addStyle"/>
        </label>
    </div>
</template>

<script>
export default {
  name: 'Input',
  props: {
    addStyle: String,
    classDiv: String,
    label: String
  }
}
</script>

<style>
    @import './Input.css';
</style>

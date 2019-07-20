<template>
<div>
  <a-menu
    style="width: 256px; height: 100%;"
    :defaultSelectedKeys="['1']"
    :defaultOpenKeys="['sub1']"
    mode="inline"
    :theme="theme"
    :selectedKeys="[current]"
    @click="handleClick"
  >
      <a-menu-item key="1"><font-awesome-icon icon="film" /><span> Filmes</span></a-menu-item>
      <a-menu-item key="2"><font-awesome-icon icon="tv" /><span> Séries</span></a-menu-item>
      <a-menu-item key="3"><font-awesome-icon icon="book"/><span> Livros</span></a-menu-item>
      <a-menu-item key="4"><font-awesome-icon icon="tv"/><span> Animações</span></a-menu-item>
  </a-menu>
      <div id="flag-mode">
        <a-switch
          defaultChecked
          @change="changeTheme"
          checkedChildren="dark"
          unCheckedChildren="light"
        />
      </div>
</div>
</template>
<script>


import { library } from '@fortawesome/fontawesome-svg-core'
import { faFilm, faTicketAlt, faBook, faTv } from '@fortawesome/free-solid-svg-icons'
library.add(faFilm, faTicketAlt, faBook, faTv)

export default {
  data () {
    return {
      current: '1',
      theme: 'dark',
    }
  },
  methods: {
    handleClick (e) {
      console.log('click ', e)
      this.current = e.key
    },
    changeTheme (checked) {
      this.theme = checked ? 'dark' : 'light'
    },
  },
}

</script>

<style>
@import url('./Menu.css');
</style>

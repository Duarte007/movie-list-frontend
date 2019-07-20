<template>
   <div class="content">
       <header>Oi</header>
        <a-button>
            Login 
            <font-awesome-icon icon="sign-in-alt" />
        </a-button>
   </div>
</template>

<script>

// import DInput from '../../components/Input/Input.vue';

import { library } from '@fortawesome/fontawesome-svg-core'
import { faSignInAlt } from '@fortawesome/free-solid-svg-icons'
library.add(faSignInAlt)

export default {
  name: 'Login',
  data(){
    return{}
  },
  props: {
    msg: String
  },
  components: {
    // DInput,
    // HelloWorld
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
@import './Login.css';
</style>

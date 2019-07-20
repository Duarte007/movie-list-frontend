<template>
<div>
  <header>Testezera</header>
  <div class="content">
    <DMenu/>
    <a-card
        style="width: 100%;"
        :tabList="tabListNoTitle"
        :activeTabKey="noTitleKey"
        @tabChange="key => onTabChange(key, 'noTitleKey')"
      >
        <p>
          <a-checkbox> 
            Avengers
          </a-checkbox> 
        </p>
        
        <p>
          <a-checkbox> 
            Avengers: Endgame
          </a-checkbox> 
        </p>
        <p>
           <a-checkbox> 
            Polar
          </a-checkbox>
        </p>
    </a-card>
  </div>
</div>
</template>

<script>

// import HelloWorld from './components/HelloWorld.vue'
// import DLogin from './components/Input/Input.vue'
// import DLogin from './components/Input/Input.vue'
import DMenu from './components/Menu/Menu.vue'
// import DCard from './components/Card/Card.vue'
// import DMenu from './app/Login/Login.vue'

export default {
  name: 'app',
  components: {
    DMenu,
    // DCard
    // DHeader,
    // HelloWorld
  },
  data(){
    return{
       tabListNoTitle: [{
        key: 'article',
        tab: 'Ação',
      }, {
        key: 'app',
        tab: 'Aventura',
      }, {
        key: 'project',
        tab: 'Comedia',
      }]
    }
  }
}
</script>

<style>
  @import './assets/css/style.css';
</style>

<template>
  <div id="app" :class="{'app-dark': darkOn}" class="app">
    <Header @onDarkMode="darkOn = $event"/>
    <Select/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Select from './components/Select.vue'

export default {
  name: 'App',
  components: {
    Header,
    Select
  },
  data(){
    return{
      darkOn: false,
    }
  },
  methods:{
     
    
  }
}
</script>

<style>
  .app {
    height: 100vh;
  }
  .app-dark{
    background: var(--very-dark-blue-bgc) ;
  }
</style>

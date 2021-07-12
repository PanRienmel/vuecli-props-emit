<template>
  <div id="app">
    <Search @ricerca="functionSearch"/>
    <Content :msg="messaggio"/>
  </div>
</template>

<script>
import Content from './components/Content.vue'
import Search from './components/Search.vue'

export default {
  name: 'App',
  components: {
    Content,
    Search
  },
  data(){
    return{
      messaggio: ""
    }
  },
  methods:{
    functionSearch(textSearch){
      this.messaggio = textSearch;
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

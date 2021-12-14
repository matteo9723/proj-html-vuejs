<template>
  <div id="app">
    <Header :dataMenu='DataHeader'/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import "@fontsource/roboto-mono";
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  data(){
    return{
      DataHeader:[
        {
          value:'home'
        },
        {
          value:'the club'
        },
        {
          value:'events'
        },
        {
          value:'../assets/img/avada-nightclub-logo.png'
        },
        {
          value:'jobs'
        },
        {
          value:'news'
        },
        {
          value:'contact us'
        }
      ]
    };
  },
  components: {
   Header,
   Main,
   Footer

  }
}
</script>

<style lang="scss" >
  *{
    font-family: "Roboto Mono";
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
</style>

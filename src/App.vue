<template>
  <div id="app">
    <Header :dataMenu='DataHeader'/>
    <Main/>
    <Footer :FirstColumnFooter='FirstColumnFooter'/>
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
      ],
      
      FirstColumnFooter:[
           {
             image:'../assets/img/avada-nightclub-events-6.jpg',
             title:'DJ Fusion',
             date:'August 19, 2022 @ 8.00 am'
           },
           {
             image:'../assets/img/avada-nightclub-events-5.jpg',
             title:'House Nation',
             date:'August 19, 2022 @ 8.00 am'
           },
           {
             image:'../assets/img/avada-nightclub-events-4.jpg',
             title:'Jazz Night',
             date:'August 19, 2022 @ 8.00 am'
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

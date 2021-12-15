<template>
  <div class="footer">
   <div class="container">
     <div class="footer-top">
       <div class="column one">
         <h4>EVENTS</h4>
         <ul>
           <li v-for="(item,index) in FirstColumnFooter" :key="index">
             <img src="../assets/img/avada-nightclub-events-6.jpg" alt="">
             <div class="text">
              <h3>{{item.title}}</h3>
              <h6>{{item.date}}</h6>
             </div>
           </li>
         </ul>
         <a href="#">View All Events</a>
       </div>
       <div class="column two">
         <img src="../assets/img/avada-nightclub-logo.png" alt="">
         <p>
           Avada nightClub
           100 Night Club Blvd
           Beverly Hills
           <a href="#">hi@your-domain.com</a>
           +1(555)000 000
         </p>
         <i class="fab fa-facebook-f"></i>
         <i class="fab fa-twitter"></i>
         <i class="fab fa-instagram"></i>
         <i class="fab fa-youtube"></i>
       </div>
       <div class="column three">
         <h4>VENUES</h4>
         <img src="../assets/img/avada-nightclub-footer-rooftop-200x86.jpg" alt="">
         <img src="../assets/img/avada-nightclub-footer-dancelounge-200x86.jpg" alt="">
       </div>
     </div>
     <div class="footer-bottom">
       <p>Copyright 2012-2021 | Avada Theme by <span> ThemeFusion</span> | All Rights Reserved | Powered by <span>Wordpress</span></p>
     </div>
   </div>
   <div class="more">
    &#8963;
   </div>
  </div>
</template>

<script>
export default {
  name:'Footer',
  props:{
    FirstColumnFooter:Array
  },
}
</script>
  
<style lang="scss" scoped>
  @import '../assets/style/general.scss';
  .footer{
    background-image: url('../assets/img/avada-nightclub-footer-background-final-2.jpg');
    background-size: cover;
    background-position: bottom;
    padding: 30px 0;
    position: relative;
    .container{
      .footer-top{
        display: flex;
        margin-bottom: 50px;

        .column{
          width: calc(100%/3);
          h4{
            color: white;
            text-align: center;
            line-height: 70px
          };
        };
        .column.one{
          ul{
            li{
              display: flex;
              align-items: center;
              margin: 30px 10px;
              img{
                width: 4vw;
                height: 4vw;
              }
              .text{
                padding: 0 10px;
                h3{
                  color: $azzurro;
                  text-align: center;
                  padding: 5px
                };
                h6{
                  color: gray;
                  text-align: center;
                  padding: 3px
                };
              };
            };
          };
          a{
            text-decoration: none;
            display: block;
            padding-left: calc(5vw + 10px);
            font-size: 12px;
            color:$azzurro;
            
          }

        };
        .column.two{
          display: flex;
          flex-wrap: wrap;
          justify-content: center;

         
          img{
            height:  70px;
         
          };
          p{
            color: gray;
            display: block;
            text-align: center;
            padding: 0 40px;
            a{
              text-decoration: none
            };
          };
          i{
            color: white;
            margin: 10px;
            cursor: pointer;
          }
          
        };
        .column.three{
          img{
            width: 100%;
            margin: 20px 0;
          }
        }
      };
      .footer-bottom{
        color: gray;
        font-size: 10px;
        text-align: center;
        
        span{
          color: $azzurro
        };
       
      };
    };
    .more{
          color: white;
          height: 30px;
          width: 30px;
          line-height: 30px;
          text-align: center;
          padding-top: 3px;         
          background-color: rgb(80, 78, 78);
          position: absolute;
          right:20px;
          bottom: 20px;      
          cursor: pointer; 
          
    }
  };
</style>
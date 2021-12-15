<template>
  <div class="header">
    <div class="container">
      <ul class="top">
       
        <li v-for="(item , index) in dataMenu " :key="index">
          <a href="#" v-if="item.value!='../assets/img/avada-nightclub-logo.png'"  >{{item.value}}</a>
          <div class="underline" v-if="item.value=='home'"></div>  
          <img src="../assets/img/avada-nightclub-logo.png" v-if="item.value=='../assets/img/avada-nightclub-logo.png'" alt="">
          
        </li>
      
      </ul>
      <div class="center">
        <img src="../assets/img/avada-nightclub-homepage-image.png" alt="">
        <h2>making memories all night long</h2>
        <div class="btn pink">become a vip</div>
      </div>
      <div class="bottom">
        <img src="../assets/img/avada-nightclub-play-showreel.png" alt="">
      </div>


    </div>
    <div class="more">
      <div class="item">
        <i class="fas fa-folder"></i>
        <span>Demos</span>
      </div>
      <div class="item">
        <div class="dollar">
          <i class="fas fa-dollar-sign"></i>
          <span>39</span>
        </div>
        <span>on sale</span>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name:'Header',
  props:{
    dataMenu:Array
  },
  methods:{
   
  }
}

</script>

<style lang="scss" scoped>
@import '../assets/style/general.scss';
  .header{
    width: 100%;
    min-height: 100vh;
    background-image: url('../assets/img/avada-nightclub-home-hero.jpg');
    background-size:cover;
    position: relative;
    .container{
      .top{
      display: flex;
      list-style-type: none;
      justify-content: space-between;
      align-items: center;
      li:first-child{
        a{
          color: $pink;
        }
      }
      li{
        margin: 10px 0px;
        position: relative;
        a{
          text-decoration: none;
          color: white;
          text-transform: uppercase;
          font-size: 12px;
        };
        .underline{
          height: 2px;
          background-color:$pink;
          position: absolute;
          width: 100%;
          bottom: -10px;
        };
        img{
          width: 250px;
         
        };
      };
      
      };  
      .center{
        position: relative;
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-top: 60px;
        img{
          width: 100%;
          min-width: 500px;
          
        };
        h2{
          border-top:5px solid $azzurro ; 
          color: white;
          background-color: rgba($color: #000000, $alpha: .3);
          padding: 50px;
          text-align: center;
          width: 100%;
          min-width: 500px;
        };
        .btn{
         position: absolute;
          bottom: 0;
          transform: translateY(50%);
        };
      };
      .bottom{
        display: flex;
        justify-content: center;
        img{
          width: 150px;
          margin: 50px 0 20px 0;
          cursor: pointer
        };
      };
    };
    .more{
      position: absolute;
      right:  10px;
      top: 100px;
      .item{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        height: 45px;
        width: 45px;
        background-color: white;
        border-radius: 5px;
        margin-bottom: 5px;
        cursor: pointer;
        span,i{
          color: #33475B;
        };
        span{
          font-size: 10px
        };
        .dollar{
          position: relative;
          i,span{
            color: rgb(42, 180, 42);
          };
          span{
            font-size: 20px
          };
          i{
            font-size: 10px;
            position: absolute;
            top: 4px;
            left: -5px;
          }
        };
      };
    };
  };
  
</style>
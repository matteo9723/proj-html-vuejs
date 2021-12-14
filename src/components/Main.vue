<template>
  <div class="main" >

    <section class="one">

      <div class="container">
       <div class="top">
         <span>welcome to avada</span>
         <h2>have the night of your life</h2>
         <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Veritatis exercitationem repellendus praesentium excepturi blanditiis consequuntur nostrum officia asperiores harum deleniti debitis maxime vitae voluptatum rerum ut, quae eaque distinctio dolor?</p>
       </div>
       <div class="bottom">
         <div class="box-images" > 
          <div class="image">
            <img src="../assets/img/avada-nightclub-dancelounge-small.jpg" alt="">
            <div class="title">
              <span class="text">dance lounge</span>
              <span class="line blue"></span>
            </div>
          </div>
          <div class="image">
            <img src="../assets/img/avada-nightclub-rooftoplounge-small.jpg" alt="">
            <div class="title">
              <span class="text">rooftop bar</span>
              <span class="line pink"></span>
            </div>
          </div>
         </div>
         <div class="box-images" >
          <div class="image">
            <img src="../assets/img/avada-nightclub-viplounge-small.jpg" alt="">
            <div class="title">
              <span class="text">vip lounge</span>
              <span class="line seppia"></span>
            </div>
          </div>
          <div class="image">
            <img src="../assets/img/avada-nightclub-events-small.jpg" alt="">
            <div class="title">
              <span class="text">resident dj</span>
              <span class="line maple"></span>
            </div>
          </div>
         </div>
         
       </div>
      </div>
   
    </section>

    <section class="two">
      <div class="image one">
       <h5>RESIDENT DJ</h5>
       <h1>dj avada</h1>
       <div class="btn blue">VIEW PROFILE</div>
      </div>
      <div class="image two">
       <h5>SPECIAL GUEST DJ</h5>
       <h1>dj blondie</h1>
       <div class="btn pink">VIEW PROFILE</div>
      </div>
    </section>

    <section class="three" >
      <div class="image-background">
      </div>
      <div class="container">
      <h4>SPECIAL EVENTS</h4>
      <h1>for you diary</h1>
        <div class="item">
          <img src="../assets/img/avada-nightclub-events-6.jpg" alt="">
          <h5>DJ Fusion</h5>
          <h6>August 19,2021@8:00 am</h6>
        </div>
        <div class="item">
          <img src="../assets/img/avada-nightclub-events-5.jpg" alt="">
          <h5>House Nation</h5>
          <h6>August 19,2021@8:00 am</h6>
        </div>
        <div class="item">
          <img src="../assets/img/avada-nightclub-events-4.jpg" alt="">
          <h5>Jazz Night</h5>
          <h6>August 19,2021@8:00 am</h6>
        </div>
        <div class="item">
          <img src="../assets/img/avada-nightclub-events-3.jpg" alt="">
          <h5>VIP Taster Sessions</h5>
          <h6>August 19,2021@8:00 am</h6>
        </div>
        <div class="item">
          <img src="../assets/img/avada-nightclub-events-2.jpg" alt="">
          <h5>Funky House Rave</h5>
          <h6>August 19,2021@8:00 am</h6>
        </div>
        <div class="item">
          <img src="../assets/img/avada-nightclub-events-1.jpg" alt="">
          <h5>Urban Vibes</h5>
          <h6>August 19,2021@8:00 am</h6>
        </div>
        <div class="btn pink">RSPV NOW</div>
      </div>
    </section>

    <section class="four" >
      <div class="box">
        <h5>BECOME A VIP TONIGHT</h5>
        <h1>exclusive vip lounge</h1>
      </div>
      <div class="box">

        <div class="btn pink">JOIN THE CLUB</div>
      </div>
    </section>
    
  </div>
</template>

<script>
export default {
  name:'Main'
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/general.scss';

  .main{
    section.one{
      background-image:url('../assets/img/avada-nightclub-cloud-background.jpg') ;
      display: flex;
      align-items: center;
      
      padding: 200px 0;
      background-size: cover;
      .container{
        .top{
          text-align: center;
          span{
            color: $azzurro;
            text-transform: uppercase;
          }
          h2{
            color: white;
          }
          p{
            color: gray;
            font-size: 12px;  
            padding:20px 50px ;
          }
        };
        .bottom{
          margin:  30px 0;
          
          
          .box-images{
            width: 100%;
            display: flex;
            flex-wrap: wrap;
            

            .image{
              width: 50%;
              position: relative;
              img{
                width: 100%;
          
              };
              .title{
                position: absolute;
                bottom: 30px;
                width: 100%;
                .text{
                  color: white;
                  width: 40%;
                  display: inline-block;
                  text-align: right;
                };
                .line{
                  width:calc(60% - 5px);
                  height: 1px;
                  margin-bottom: 6px;
                  margin-left: 5px;
                  background-color: $azzurro;
                  display: inline-block
                };
                .line.blue{
                  background-color: $azzurro;
                };
                .line.pink{
                  background-color: $pink;
                };
                .line.seppia{
                  background-color: $seppia;
                };
                .line.maple{
                  background-color: $maple;
                };
              };
            };
          };
          .box-images:last-child{
            margin-top: -4px;
          }
        };
      };
    };
    section.two{
      display: flex;
      flex-wrap: wrap;
      .image{
        width: 50%;
        height: 500px;
        background-size: cover;
        position: relative;
        padding:50px 30px;
        h5{
          color: $pink;
          margin: 10px
        };
        h1{
          color: white;
          margin:10px;
        };
        .btn{
          margin: 10px;
          position: absolute;
        }
      };
      .image.one{
        background-image: url('../assets/img/avada-nightclub-resident-profile.jpg');
        background-position: center;
        border-top: 5px solid $pink;
        h5{
          color: $pink;
        };
      };
      .image.two{
        background-image: url('../assets/img/avada-nightclub-lisahouse-inset-new.jpg');
         border-top: 5px solid $azzurro;
        h5{
          color: $azzurro;
        };
      };
    };
    section.three{
     position: relative;
     height: 1000px;
     
     
      .image-background{
        background-image: url('../assets/img/avada-nightclub-homepage-events-background-new.jpg');
        background-size: cover;
        background-position: center;
        height: 1000px;
        width: 100%;
        position: absolute;
        filter: brightness(20%);

      };
      .container{
        display: flex;
        flex-wrap: wrap;
        position: absolute;
        left:50%;
        top:50%;
        transform: translate(-50%,-50%);
        h1,h4{
          text-align: center;
          width: 100%;
        };
        h1{
          color: white;
          margin-bottom: 20px;
        };
        h4{
          color:$pink;
          font-size: 12px
        };
        .item{
          width: calc(100% / 3 - 20px);
          margin: 30px 10px;
          h5,h6{
            padding:0 10px;
          };
          h5{
            color: $pink;
          };
          h6{
            color: white;
          };
          img{
            width: 100%;
          };
        };
        .btn.pink{
          position: absolute;
          bottom: -30px;
          left: 50%;
          transform: translateX(-50%)
        }
      };
    };
    section.four{
      background-image: url('../assets/img/avada-nightclub-vip-hero-new.jpg');
      height: 250px;
      background-size: cover;
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: center;

      .box{
        position: relative;
        padding-left: 100px;
        h1{
          color: white;
        };
        h5{
          color: $azzurro;
        };
      };
    };
  };

</style>
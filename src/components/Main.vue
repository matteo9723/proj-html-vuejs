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
              <span class="line"></span>
            </div>
          </div>
          <div class="image">
            <img src="../assets/img/avada-nightclub-rooftoplounge-small.jpg" alt="">
          </div>
         </div>
         <div class="box-images" >
          <div class="image">
            <img src="../assets/img/avada-nightclub-viplounge-small.jpg" alt="">
          </div>
          <div class="image">
            <img src="../assets/img/avada-nightclub-events-small.jpg" alt="">
          </div>
         </div>
         
       </div>
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
                  width: 60%;
                  height: 2px;
                  background-color: $azzurro;
                  display: inline-block
                }
              }
            };
          };
          .box-images:last-child{
            margin-top: -4px;
          }
        };
      };
    }
  };

</style>
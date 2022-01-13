<template>
  <footer>
    <div class="topFooter container d-flex justify-content-between align-items-center">
      <div class="col-3">
        <img src="../../assets/img/avada-drivers-logo-2x-300x58.png" alt="">
        <div class="text mt-2">Avada Driving School is the right choice for experienced drivers looking for a refresher course, or the brand new driver wanting to pass first time.</div>
      </div>
      <div class="containerList d-flex">
        <div class="col-6 ">
          <div class="titleSection">CONTACT DETAILS</div>
          <ul class="detail">
            <li>
              <i class="fas fa-home"></i>
              <span>12345 North Main Street, New York, NY 555555</span>
            </li>

            <li>
              <i class="fas fa-phone"></i>
              <span>1.800.555.6789</span> 
            </li>
            <li>
              <i class="far fa-envelope"></i>
              <span>info@your-domain.com</span>
            </li>
            <li>
              <i class="fas fa-link"></i>
              <span>Theme-Fusion.com</span>
            </li>
          </ul>
        </div>

        <div class="col-6">
          <div class="titleSection">COURSES</div>
          <ul>
            <courses v-for="(item, index) in courses" :key="index" :contact="item"/>
          </ul>
        </div>
      </div>


      <div class="col-3 grid d-flex flex-column align-items-center">
        <img src="../../assets/img/grid.png" alt="">
        <div class="btnGreen">book now</div>
      </div>
    </div>
    <div class="bottomFooter">
      <div class="container h-100 d-flex align-items-center justify-content-between">
        <div class="copyrigth">© Copyright 2012 - 2022 | Avada Theme by <a href="">ThemeFusion</a>  | All Rights Reserved | Powered by <a href="">WordPress</a></div>
        <div class="SocialMedia">
          <span><i class="fab fa-facebook-f"></i></span>
          <span><i class="fab fa-twitter"></i></span>
          <span><i class="fab fa-youtube"></i></span>
          <span><i class="fab fa-instagram"></i></span>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>

import courses from '../elements/courses.vue';

export default {
    name: 'Footer',

    components:{
      courses,
    },

    data(){
      return{
        courses:[
        {
          course:'Pass Plus',
        },
        {
          course:'Intensive Course',
        },
        {
          course:'Automatic',
        },
        {
          course:'Instructor Training',
        }],
      }
    },

}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

  footer{
    height: 600px;
    background-image: url('../../assets/img/footer-background-color.jpg');
    background-size: cover;
    background-position: center;
  }
  a{
    color: $primaryColor
  }
  .topFooter{
    height: 450px;
  }

  .text{
    color: $primaryColorText;
    line-height: 2rem;
  }
  .titleSection{
    text-align: center;
    color: white;
    font-weight: bold;
    font-size: 20px;
  }
  .detail li{
    margin: 15px;
    color: $primaryColorText;
  }
  .detail span{
    margin-left: 20px;
  }

  .grid img{
    width: 80%;
    margin-bottom: 20px;
  }

  ul li i{
    display: inline;
    margin-right: 20px;
  }
  .bottomFooter{
    height: 150px;
    background-color: #0f1d1f;
    color: $primaryColorText;
  }

  .copyrigth{
    font-size: 14px;
  }


  .bottomFooter span {
    color: white;
    margin-right: 20px;
    font-size: 20px;
  }

</style>
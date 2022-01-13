<template>
  <div class="card">
      <img src="../../assets/img/instructor-mikehart-400x254.jpg" alt="">
      <div class="name">Mike Hart</div>
      <div class="socialMedia">
          <span><i class="fab fa-facebook-f"></i></span>
          <span><i class="fab fa-twitter"></i></span>
          <span><i class="fab fa-instagram"></i></span>
      </div>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
  </div>
</template>

<script>
export default {
    name: 'cardInstructors'
}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

.card{
    margin-top: 60px;;
    width: 400px;
    height: 460px;
    padding: 50px;
    border-top: 6px solid $primaryColor;
    text-align: center;
    border-radius:  .5rem;
    box-shadow: 10px 10px 45px -8px rgba(0,0,0,0.20);
}

.name{
    font-size: 26px;
    font-weight: 600;
    margin: 30px 0px 10px 0px;
}

.socialMedia{
     font-size: 20px;
     color: $primaryColorText;

     & span{
         margin: 10px ;
     }
}

p{
    color: $primaryColorText;
    margin-top: 10px;
    line-height: 2rem;
}

</style>
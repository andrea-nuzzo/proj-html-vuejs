<template>
  <div class="card">
      <img :src="instructorData.img" :alt="instructorData.name">
      <div class="name">{{instructorData.name}}</div>
      <div class="socialMedia">
          <span><i class="fab fa-facebook-f"></i></span>
          <span><i class="fab fa-twitter"></i></span>
          <span><i class="fab fa-instagram"></i></span>
      </div>
      <p>{{instructorData.description}}</p>
  </div>
</template>

<script>
export default {
    name: 'cardInstructors',

    props:{
        instructorData: Object
    },

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
    cursor: pointer;
    
}

.mouseHover{
    position: relative;
    top: -30px;
    width: 60%;
    margin: 0 auto;
    border-radius: 2rem;
    color: white;
    background-color: $primaryColor;
}
.card:hover{
    transform: scale(1.1);
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
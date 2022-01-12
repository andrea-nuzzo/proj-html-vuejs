<template>
  <div class="card">
    <img src="../../assets/img/new-corner.jpg" alt="">
    <h2 class="title">Courses</h2>
    <p class="text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper.</p>
    <div class="btnGreen">Course Information</div>

  </div>
</template>

<script>
export default { 
    name: 'cardCourses'
}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

.card{
    width: 400px;
    padding: 50px;
    text-align: center;
    border: none;
    border-radius:  .5rem;
    box-shadow: 10px 10px 45px -8px rgba(0,0,0,0.20);
    position: relative;
}
img{
    width: 80px;
    border-top-left-radius: .5rem;
    position: absolute;
    top: 0;
    left: 0;
}

p{
    color: $primaryColorText ;
    line-height: 2rem;
}

.text{
    margin: 40px 0;
}

.btnGreen{
    width: 80%;
    margin: 0 auto;
}

</style>
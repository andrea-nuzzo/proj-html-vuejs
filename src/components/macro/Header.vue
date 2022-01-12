<template>
  <header>
    <div class="topHeader">
      <div class="left">
        <span>We have a 95% Successful Pass Rate!</span>
      </div>
      <div class="rigth">
        <i class="fas fa-phone"></i>
        <span>Give us a call to book your tuition! 1-800-555-555</span>
      </div>
    </div>
    
  </header>
</template>

<script>
export default {
    name: 'Header',

}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

header{
    height: 750px;
    background-image: url('../../assets/img/homepage-hero-background.jpg');
    background-position: center;
    background-size: cover;
}

.topHeader{
  background-color: $topHeaderColor;
  color: #7f9ea8;
  font-size: 12px;
  height: 40px;

  display: flex;
  justify-content: space-around;
  align-items: center;
}
.fa-phone{
  margin-right: 10px;  
}

</style>
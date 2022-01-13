<template>
  <header>

    <div class="topHeader d-flex align-items-center">
      <div class="container d-flex justify-content-between">
        <div class="left">
          <span>We have a 95% Successful Pass Rate!</span>
        </div>
        <div class="rigth">
          <i class="fas fa-phone "></i>
          <span class="ms-3">Give us a call to book your tuition! 1-800-555-555</span>
        </div>
      </div>
    </div>

    <div class="backgroundNavbar">
      <div class="container d-flex justify-content-between align-items-center pt-4 pb-4">

        <div class="logo">
          <img src="../../assets/img/avada-drivers-logo-2x-300x58.png" alt="logo">
        </div>

        <div class="navbar">
          <nav>
            <li><a href="#">home</a></li>
            <li><a href="#">about</a></li>
            <li><a href="#">prices</a></li>
            <li><a href="#">courses</a></li>
            <li><a href="#">locations</a></li>
            <li><a href="#">blog</a></li>
            <li><button class="btnGreen">book now</button></li>
          </nav>
        </div>        
      </div>      
    </div>
    
    <div class="title">
      <div class="container d-flex flex-column justify-content-center h-100">
          <h1>Drive with Avada</h1>
          <h2>We offer the finest driving tuition money can buy</h2>
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

}

.backgroundNavbar{
  background-color: rgba($color: #353637, $alpha: 0.5);
}


li{
    text-transform: uppercase;
    display: inline;
    margin: 20px;

  & a{
    color: #ffffff;
  }
}

a:hover{
  color: $primaryColor;
  
}

li:hover:not(:last-child){
  border-bottom: 5px solid $primaryColor;
  padding-bottom: 10px;
}

.title {
  height: 602px;
}

.container{
  & h1, h2{
    color:white
    
  }

  & h1{
    font-size: 65px;
    font-weight: bold;
    margin-bottom: 15px;
  }

  & h2{
    font-size: 28px;
    font-weight: 300;
  }
} 

</style>
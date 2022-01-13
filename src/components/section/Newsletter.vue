<template>
  <div class="background">
      <div class="container h-100 d-flex flex-column justify-content-center align-items-center">
        <div class="title">Sign up to our Newsletter</div>
        <input type="text">
        <div class="btnGreen">subscribe</div>
        <div class="alert">(We do not share your data with anybody, and only use it for its intended purpose)</div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Newsletter',
}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

.background{
    height: 400px;
    background-image: url('../../assets/img/newsletter_background.jpg');
    background-position: center;
    background-size: cover;
}
input{
    background-color: #f7f7f7;
    border: 1px solid #e5e8eb ;
    padding: 10px;
    border-radius:  .5rem;
    margin: 30px 0px 30px 0px;
}

.btnGreen, input{
    width: 50%;
}

.btnGreen{
    margin-bottom: 30px;
}

.alert{
    color: $primaryColorText;
    font-size: 14px;
}

</style>
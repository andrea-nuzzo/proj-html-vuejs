<template>
  <div class="background">
      <div class="container d-flex flex-column justify-content-center align-items-center">
        <div class="title">Testimonials</div>
        <div class="subTitle">Here’s what our happy drivers had to say about our services:</div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Testimonials',
}
</script>

<style lang="scss" scoped>
    .background{
        height: 1000px;
        background-image: url('../../assets/img/testimonial-background.jpg');
        background-position: center;
        background-size: cover;
    }
.container{
    height: inherit;
}
</style>
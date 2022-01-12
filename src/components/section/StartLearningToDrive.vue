<template>
  <div class="backgroundSection">
      <div class="container d-flex justify-content-between align-items-center h-100">
          <div class="left">
              <div class="title">Start Learning to Drive Today</div>
              <div class="subTitle">Give us a call to schedule your first driving lesson</div>
          </div>
          <div class="rigth">
              <i class="fas fa-phone"></i>
              <span class="ms-4">1-800-555-555</span>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'StartLearningToDrive'
}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

.backgroundSection{
    height: 250px;
    background-image: url('../../assets/img/horizontal-cta-background.jpg');
    background-position: center;
    background-size: cover;
    color: white;
}
.rigth{
    font-size: 35px;
    font-weight: 300;
}
</style>
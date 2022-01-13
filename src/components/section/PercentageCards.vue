<template>
  <div class="container d-flex justify-content-between">
      <card95 class="move"/>
      <card100 class="move"/>
      <card0 class="move"/>
  </div>
</template>

<script>
import card95 from '../elements/card95.vue';
import card100 from '../elements/card100.vue';
import card0 from '../elements/card0.vue'
export default {
    name: 'PercentageCards',

    components:{
        card95,
        card100,
        card0,
    }
}
</script>

<style lang="scss" scoped>
    .move{
        top: 300px;
    }
</style>
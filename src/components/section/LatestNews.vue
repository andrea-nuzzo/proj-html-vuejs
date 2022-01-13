<template>
  <div class="background">
    <latestCard class="move"/>
  </div>
</template>

<script>
import latestCard from '../elements/latestCard.vue'
export default {
    name: 'LatestNews',

    components:{
        latestCard,
    },
}
</script>

<style lang="scss" scoped>

    .background{
        height: 900px;
        background-image: url('../../assets/img/latestnews-background.jpg');
        background-position: center;
        background-size: cover;
    }

    .move{
        top: -50px;
        margin: 0 auto;
    }

</style>
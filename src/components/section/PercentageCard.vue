<template>
<div class="container">
    <card95/>
</div>
</template>

<script>
import card95 from '../elements/card95.vue'

export default {
    name: 'PercentageCard',

    components:{
        card95,
    }
}
</script>

<style lang="scss" scoped>
    .container{
        background-color: greenyellow;
    }
</style>
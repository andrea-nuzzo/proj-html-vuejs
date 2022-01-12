<template>
<div class="container d-flex justify-content-between align-items-center">
    <div class="left">
        <h2>Get Behind The Wheel</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper.</p>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper. Fusce et ultrices libero, at suscipit lacus. Sed vitae fringilla nibh. Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper. Fusce et ultrices libero, at suscipit lacus. Sed vitae fringilla nibh.</p>
    </div>
    <div class="rigth">
        <cardRequest/>
    </div>
</div>
</template>

<script>
import cardRequest from '../elements/cardRequest.vue';
export default {
name: 'GetBehindTheWheel',

components:{
    cardRequest,
}

}
</script>

<style lang="scss" scoped>



</style>
<template>
<div class="container d-flex justify-content-between">
    <div class="left">
        <h2 class="title">Get Behind The Wheel</h2>
        <p class="subTitle">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper.</p>
        <p class="text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper. Fusce et ultrices libero, at suscipit lacus. Sed vitae fringilla nibh. Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper. Fusce et ultrices libero, at suscipit lacus. Sed vitae fringilla nibh.</p>
    </div>
    <div class="rigth">
        <cardRequest class="move"/>
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

@import '../../assets/style/partials/variables.scss';

h2{
    margin: 80px 0px 30px 0px;
}
.subTitle, .text{
    color: $primaryColorText ;
    line-height: 2rem;
    margin-right: 90px ;
}

.move{
    top: -50px;
}
</style>
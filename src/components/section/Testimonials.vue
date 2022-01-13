<template>
    <div class="background">
        <div class="container d-flex flex-column justify-content-center align-items-center">
            <div class="title">Testimonials</div>
            <div class="subTitle">Here’s what our happy drivers had to say about our services:</div>

            <img src="../../assets/img/testimonial-sophia.png" alt="">

            <div class="text">Avada Driving School really helped build my confidence behind the wheel and with driving in general, and they got me a first time pass! Highly recommended.</div>

            <div class="name">Sophia Jones</div>
            
            <div class="dot">
                <i class="fas fa-circle"></i>
                <i class="far fa-circle"></i>
                <i class="far fa-circle"></i>
                <i class="far fa-circle"></i>
                <i class="far fa-circle"></i>
            </div>
            <carousel/>
        </div>
    </div>
</template>

<script>

export default {
    name: 'Testimonials',

}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
    .background{
        height: 900px;
        background-image: url('../../assets/img/testimonial-background.jpg');
        background-position: center;
        background-size: cover;
    }

    .subTitle, .text, .name, .dot{
        color: $primaryColorText;
    }

    .subTitle{
        margin-bottom: 50px;
    }
    .text{
        font-size: 18px;
        text-align: center;
        line-height: 2rem;
        width: 50%;
    }

    .name{
        margin: 30px 0;
        font-size: 18px;
        font-weight: bold;
    }

    .fa-circle{
        font-size: 14px;
    }

    .fa-circle:not(:first-child){
        margin-left: 15px;
    }

    img{
        width: 180px;
        margin-bottom: 30px;
    }


    .container{
        height: inherit;
    }
</style>
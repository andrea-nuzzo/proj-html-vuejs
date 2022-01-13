<template>
    <div class="card">
        <div class="title">Latest News</div>
        <div class="containerSection d-flex">

            <div class="left">
                <img src="../../assets/img/blog-choosecar-700x441.jpg" alt="">
                <div class="newsTitle">What Car to Start With?</div>
                <div class="date">
                     <span>February 7th, 2019 | </span>
                      <span> 0 Comments</span>
                </div>
                <div class="text">Lorem ipsum dolor sit amet, consectetur adipiscing</div>
            </div>

            <div class="rigth">
                <img src="../../assets/img/blogpost-10and2-700x441.jpg" alt="">
                <div class="newsTitle">Avada Driving School Expanding</div>
                <div class="date">
                    <span>February 7th, 2019 | </span>
                    <span> 0 Comments</span>
                </div>
                <div class="text">Lorem ipsum dolor sit amet, consectetur adipiscing</div>
            </div>            
        </div>
        <div class="btnGreen">more from the blog</div>
        <img src="../../assets/img/latestnews-bottom-1200x105.png" alt="">
    </div>
</template>

<script>
export default {
    name: 'latestCard'
}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

   .card{
    width: 60%;
    height: 80%;
    padding: 50px;
    border-top: 6px solid $primaryColorText;
    text-align: center;
    border-top-left-radius:  .5rem;
    border-top-right-radius: .5rem;
    box-shadow: 10px 10px 45px -8px rgba(0,0,0,0.20);
    position: relative;
}

.title{
    margin-bottom: 50px;
}

img{
    width: 90%;
}

.newsTitle{
    font-size: 22px;
    font-weight: bold;
    color: $primaryColor;
    margin-top: 20px;
}
.date{
    color: $primaryColor;
    font-size: 14px;
    margin-bottom: 30px;
}

span:first-child, .text{
    color: $primaryColorText
}

.btnGreen{
    width: 20%;
    margin: 50px auto;
}

img:last-child{
    width: 100%;
    position: absolute;
    bottom: -111px;
    right: 0;
}

</style>
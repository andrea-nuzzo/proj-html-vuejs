<template>
<div>
    <div class="background">
        <div class="container d-flex justify-content-between">
            <div class="left">
                <cardCourses class="move"/>
            </div>
            <div class="rigth d-flex justify-content-around align-items-center">
                <div class="typeOfCourses" v-for="(item, index) in typeCourses" :key="index" >
                    <img :src="item.img" alt="">
                    <div class="subTitle">{{item.text}}</div>
                    <div class="btnGray">learn more</div>
                </div>
            </div>
        </div>
    </div>
    <div class="triangle">
        <img src="../../assets/img/driving-triangle.svg" alt="">
    </div>

</div>
</template>

<script>
import cardCourses from '../elements/cardCourses.vue'
export default {
name: 'GetBehindTheWheel',

components:{
    cardCourses,
},

data () {
    return{
        typeCourses:[
            {
                img:require('../../assets/img/courses-passplus-400x399.jpg'),
                text:'Pass Plus'
            },
            {
                img:require('../../assets/img/course-intensive-400x399.jpg'),
                text:'Intensive Course'
            },
             {
                img:require('../../assets/img/courses-instructor-400x400.jpg'),
                text:'Instructors'
            },
        ]
    }
},

}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

.background{
    position: absolute;
    height: 480px;
    width: 100%;
    background-image: url('../../assets/img/promise-background.jpg');
    background-position: bottom;
    background-size: cover;
}
.move{
    top: -30px
}
.rigth{
    height: inherit;
    width: 100%;
}
.triangle img{  
    position: relative;
    left: 0;
    bottom: -479px; 
    width: 100%;
    height: 100px
}
.typeOfCourses img{
    width: 180px;
}

.subTitle{
    text-align: center;
    font-size: 18px;
    color: $primaryColorText;
    font-weight: bold;
    margin: 20px 0px 10px 0px;

}

.btnGray{
    width: 70%;
    font-size: 10px;
    text-align: center;
    margin: 0 auto;
}

</style>
<template>
  <div>
      <div class="container">
        <div class="title col-12">
            <h2 class="title">Your Instructors</h2>
        </div>
        <div class="d-flex align-items-center">
            <div class="rigth col-7">
                <div class="subTitle">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper.</div>
            </div>
            <div class="left col-5">
                <div class="btnGreen">more about us</div>
            </div>
        </div>
        <div class="d-flex justify-content-between">
            <cardInstructors class="move" v-for="(instructor, index) in instructors" :key="index" :instructorData="instructor"/>
        </div>
      </div>
  </div>
</template>


<script>
import cardInstructors from '../elements/cardInstructors.vue'
export default {
    name: 'Istructors',

    components:{
        cardInstructors,
    },

    data(){
        return{
            instructors:[
                {
                    name: 'Mike Hart',
                    img: require('../../assets/img/instructor-mikehart-400x254.jpg'),
                    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
                },
                {
                    name: 'John Smith',
                    img: require('../../assets/img/instructor-johnsmith-400x254.jpg'),
                    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
                },
                {
                    name: 'Angela Hart',
                    img: require('../../assets/img/instructor-angelahart-400x254.jpg'),
                    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
                },
            ],
        }
    },
}
</script>




<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

.title{
    margin-top: 400px;
}

h2{
    margin: 80px 0px 30px 0px;
}

.subTitle{
    color: $primaryColorText ;
    line-height: 2rem;
}

.btnGreen {
    width: 75%;
}
.move{
    bottom: -70px;
}

</style>
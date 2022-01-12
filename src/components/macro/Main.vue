<template>
  <main>
    <GetBehindTheWheel/>
    <StartLearningToDrive/>
    <Courses/>
    <Istructors/>
    <Testimonials/>
    <LatestNews/>
    <Newsletter/>
  </main>
</template>

<script>
import GetBehindTheWheel from '../section/GetBehindTheWheel.vue';
import StartLearningToDrive from'../section/StartLearningToDrive.vue';
import Courses from'../section/Courses.vue';
import Istructors from'../section/Istructors.vue';
import Testimonials from'../section/Testimonials.vue';
import LatestNews from'../section/LatestNews.vue';
import Newsletter from'../section/Newsletter.vue';

export default {
    name: 'Main',
    components:{
      GetBehindTheWheel,
      StartLearningToDrive,
      Courses,
      Istructors,
      Testimonials,
      LatestNews,
      Newsletter,
    }

}
</script>

<style lang="scss" scoped>

</style>
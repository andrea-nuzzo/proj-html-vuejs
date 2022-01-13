<template>
  <div>
      <li>
          <i class="far fa-arrow-alt-circle-right"></i>
          <a href="">{{contact.course}}</a>
      </li>
  </div>
</template>

<script>
export default {
    name: 'courses',

    props: {
        contact: Object,
    },

}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

a:hover{
   color: inherit;
}

li, a {
    color: $primaryColor;
}

li{
    margin: 15px
}

.fa-arrow-alt-circle-right{
    margin-right: 20px;
}

</style>
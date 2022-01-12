<template>
  <div class="card">
    <h2 class="mb-4">First Lesson Free!</h2>
    <p>When you make a block booking with us your first lesson is included free.</p>
    <input type="text" placeholder="Your Name*">
    <input type="email" placeholder="Email*">
    <input type="tel" placeholder="Thelephone">
    <input type="text" placeholder="Location">
    <div class="btnGreen">request a callback</div>

  </div>
</template>

<script>
export default { 
    name: 'cardRequest'
}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

.card{
    width: 550px;
    padding: 50px;
    text-align: center;
    border: none;
    border-radius:  .5rem;
    box-shadow: 10px 10px 45px -8px rgba(0,0,0,0.20);
}
h2{
    color: $primaryColor;
    font-weight: bold;
}

p{
    color: $primaryColorText ;
    font-size: 14px;
    line-height: 2rem;
}
input{
    margin: 0 auto;
    width: 100%;
    background-color: #f7f7f7;
    border: 1px solid #e5e8eb ;
    padding: 10px;
    border-radius:  .5rem;
    margin-bottom: 30px;
}

::placeholder{
    color: $primaryColorText;
    font-size: 12px;
}
.btnGreen{
    width: 50%;
    margin: 0 auto;
}

</style>
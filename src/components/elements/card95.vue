<template>
  <div class="card d-flex flex-column align-items-center">
    <div class="test">
      <svg class="d-flex justify-content-center">
        <circle cx="100" cy="100" r="100" />
        <circle cx="100" cy="100" r="100" />
      </svg>
      <div>95%</div>
      <div>PASS RATE</div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'card95',


}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

.card{
    margin-top: 60px;;
    width: 400px;
    height: 460px;
    padding: 50px;
    border-top: 6px solid $primaryColor;
    text-align: center;
    border-radius:  .5rem;
    box-shadow: 10px 10px 45px -8px rgba(0,0,0,0.20);
    cursor: pointer;
    
}

.test {
	width: 100%;
	height: 100%;
}

svg {
	width: 100%;
	height: 100%;
}

.test circle {
	transform: rotate(-90deg) translate(10px, 10px);
	transform-origin: center;
	fill: none;
	stroke: #ddd;
	stroke-width: 8px;
	stroke-linecap: round;
}

.test circle:nth-child(2) {
	stroke: $primaryColor;
	stroke-dasharray: 750;
	stroke-dashoffset: 160;
}






</style>
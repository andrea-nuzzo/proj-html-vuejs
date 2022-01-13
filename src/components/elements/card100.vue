<template>
  <div class="card">
    <div class="test">
      <svg class="h-100">
        <circle cx="100" cy="100" r="100" />
        <circle cx="100" cy="100" r="100" />
      </svg>
      <div class="pecentage">100%</div>
      <div class="typePecentage">REFERRAL RATE</div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'card100',


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

.pecentage{
  color: $primaryColorText;
  font-size: 50px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.typePecentage{
  color: $primaryColorText;
  position: absolute;
  top: 350px;
  left: 50%;
  transform: translate(-50%,0);
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
  position: absolute;
	transform: rotate(-90deg);
	transform-origin: center;
	fill: none;
	stroke: #ddd;
	stroke-width: 8px;
	stroke-linecap: round;
}

.test circle:nth-child(2) {
	stroke: $primaryColor;
	stroke-dasharray: 800;
	stroke-dashoffset: 160;
}









</style>
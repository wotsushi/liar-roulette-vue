<template>
  <div style="animation: rotate-anime 3s linear infinite">
    <wheel/>
  </div>

</template>

<script>
import Wheel from './Wheel.vue'

export default {
  components: {
    Wheel
  }
}
</script>

<style>
@keyframes rotate-anime {
  0%  {transform: rotate(0);}
  100%  {transform: rotate(360deg);}
}
</style>
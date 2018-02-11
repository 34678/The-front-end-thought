<template lang="html">
    <div>
        <heador></heador>
        <h-slider></h-slider>
        <novice></novice>
        <borrow></borrow>
        <money></money>
        <product></product>
        <life></life>
    </div>
</template>

<script>
  import Heador from '../public/header'
  import HSlider from '../home/hslider'
  import Novice from '../home/novice'
  import Borrow from '../home/borrow'
  import Money from '../home/money'
  import Life from '../home/life'
  import Product from '../home/product'

  export default {
    components: {
      Heador,
      HSlider,
      Novice,
      Borrow,
      Money,
      Life,
      Product
    }
  }
</script>

<style lang="scss" module>
    @import '../../css/reset.scss';
</style>

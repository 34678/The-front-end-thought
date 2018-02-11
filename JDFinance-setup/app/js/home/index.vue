<template lang="html">
    <div>
        <heador></heador>
        <h-slider></h-slider>
        <novice></novice>
        <borrow></borrow>
        <money></money>
        <product></product>
        <life></life>
        <footor></footor>
        <navbar></navbar>
    </div>
</template>

<script>
  import Heador from '../public/header'
  import Navbar from '../public/navbar'
  import Footor from '../public/footer'
  import HSlider from '../home/hslider'
  import Novice from '../home/novice'
  import Borrow from '../home/borrow'
  import Money from '../home/money'
  import Life from '../home/life'
  import Product from '../home/product'

  export default {
    components: {
      Navbar,
      Heador,
      HSlider,
      Novice,
      Borrow,
      Money,
      Life,
      Product,
      Footor
    }
  }
</script>

<style lang="scss" module>
    @import '../../css/reset.scss';
</style>

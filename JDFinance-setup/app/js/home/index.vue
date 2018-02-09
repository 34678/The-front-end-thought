<template lang="html">
    <div>
        <heador></heador>
        <h-slider></h-slider>
        <novice></novice>
        <borrow></borrow>
        <money></money>
    </div>
</template>

<script>
  import Heador from '../public/header'
  import HSlider from '../home/hslider'
  import Novice from '../home/novice'
  import Borrow from '../home/borrow'
  import Money from '../home/money'

  export default {
    components: {
      Heador,
      HSlider,
      Novice,
      Borrow,
      Money
    }
  }
</script>

<style lang="scss" module>
    @import '../../css/reset.scss';

    .home {
        color: blue;
        font-size: 80px;
    }
</style>

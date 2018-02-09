<template lang="html">
    <div>
        <heador></heador>
        <h-slider></h-slider>
        <novice></novice>
    </div>
</template>

<script>
  import Heador from '../public/header'
  import HSlider from '../home/hslider'
  import Novice from '../home/novice'

  export default {
    components: {
      Heador,
      HSlider,
      Novice
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

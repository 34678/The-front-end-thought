<template lang="html">
    <div>
        <heador></heador>
        <h-slider></h-slider>
    </div>
</template>

<script>
  import Heador from '../public/header'
  import HSlider from '../home/hslider'

  export default {
    components: {
      Heador,
      HSlider
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

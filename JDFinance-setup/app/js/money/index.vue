<template lang="html">
    <div>
        <heador></heador>

        <footor></footor>
        <navbar></navbar>
    </div>
</template>

<script>
  import Heador from '../public/header'
  import Navbar from '../public/navbar'
  import Footor from '../public/footer'
  import MSlider from '../money/mslider'

  export default {
    components: {
      Navbar,
      Heador,
      MSlider,
      Footor
    }
  }
</script>

<style lang="scss" module>
    @import '../../css/reset.scss';
</style>

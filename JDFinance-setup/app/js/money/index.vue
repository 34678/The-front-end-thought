<template lang="html">
    <div>
        <heador></heador>
        <m-slider></m-slider>
        <ada></ada>
        <money></money>
        <adb></adb>
        <finance></finance>
        <adc></adc>
        <footor cname="mfooter"></footor>
        <navbar></navbar>
    </div>
</template>

<script>
  import Heador from '../public/header'
  import Navbar from '../public/navbar'
  import Footor from '../public/footer'
  import MSlider from '../money/mslider'
  import Ada from '../money/ada'
  import Adb from '../money/adb'
  import Adc from '../money/adc'
  import Finance from '../money/finance'
  import Money from '../money/money'
  export default {
    components: {
      Navbar,
      Heador,
      MSlider,
      Footor,
      Ada,
      Adb,
      Adc,
      Finance,
      Money
    }
  }
</script>

<style lang="scss">
    .mfooter{
        margin-top: 0!important;
        ul{
            li:first-child{
                display: none;
            }
        }
    }
</style>

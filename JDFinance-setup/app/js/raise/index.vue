<template lang="html">
    <div>
        <heador></heador>
        <r-slider></r-slider>
<daily></daily>
        <in></in>
        <more></more>
        <footor cname="mfooter"></footor>
        <navbar></navbar>
    </div>
</template>

<script>
  import Heador from '../public/header'
  import Navbar from '../public/navbar'
  import Footor from '../public/footer'
  import RSlider from '../raise/rsilder'
  import Daily from '../raise/daily'
  import In from '../raise/in'
  import More from '../raise/more'
  export default {
    components: {
      Navbar,
      Heador,
      RSlider,
      Daily,
      In,
      More,
      Footor
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

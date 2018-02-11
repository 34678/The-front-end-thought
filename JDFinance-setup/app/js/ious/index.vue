<template lang="html">
    <div>
        <heador></heador>
<islider></islider>
        <welfare>

        </welfare>
        <service></service>
        <footor></footor>
        <navbar></navbar>
    </div>
</template>

<script>
  import Heador from '../public/header'
  import Navbar from '../public/navbar'
  import Footor from '../public/footer'
  import Islider from '../ious/islider'
  import Welfare from '../ious/welfare'
  import Service from '../ious/service'

  export default {
    components: {
      Navbar,
      Heador,
      Footor,
      Islider,
      Welfare,
      Service

    }
  }
</script>



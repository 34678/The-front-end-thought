<template lang="html">
    <div>
        <heador></heador>
    </div>
</template>

<script>
  import Heador from '../public/header'

  export default {
    components: {
      Heador
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

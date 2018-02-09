<template lang="html">
    <section :class="[panelClass,cname]">
        <h4>--{{title}}--</h4>
        <div>
            <slot></slot>
        </div>
    </section>
</template>

<script>
  export default {
    props: {
      cname: {
        type: String,
        default: ''
      },
      title: {
        type: String,
        default: ''
      }
    },
    data() {
      return {
        panelClass: 'btn'
      }
    }
  }
</script>
<style lang="css">
    @import "../../css/element.scss";

    .panel {
    @include panel
    }
</style>

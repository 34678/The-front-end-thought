<template lang="html">
    <div :class="[btnClass,cname]">
        <slot></slot>
    </div>
</template>

<script>
  // 允许自定义类 可以自定义文本
  export default {
    props: {
      cname: {
        type: String,
        default: ''
      }
    },
    data() {
      return {
        btnClass: 'btn'
      }
    }
  }
</script>
<style lang="scss">
    /*这里使用sass的btn样式*/
    @import "../../css/element.scss";
    .btn {
      @include btn
    }
</style>

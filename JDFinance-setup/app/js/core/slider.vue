<template lang="html">
    <div>
        <section :class="cname">
            <swiper :options="options" :no-next-tick="options.noNextTick">
                <swiper-slide v-for="item in items" :key="item.href">
                    <router-link :to="{name:item.href}">
                        <img :src="item.src" alt="">
                    </router-link>
                </swiper-slide>
                <div class="swiper-pagination" vif="options.pagination"></div>
            </swiper>
        </section>
    </div>
</template>

<script>
  import {swiper, swiperSlide} from 'vue-awesome-swiper'

  export default {
    components: {
      swiperSlide,
      swiper
    },
    props: {
      cname: {
        type: String,
        default: ''
      },
      options: {
        type: Object,
        default() {
          return {
            autoplay: true,
            loop: true,
            pegination: {
              el: '.swiper-pagination',
            },
            notNextTick: false
          }
        }
      },
      item: {
        type: Array,
        default() {
          return []
        }
      }
    }
  }
</script>
<style lang="css">
    @import "~swiper/dist/css/swiper.css";
</style>

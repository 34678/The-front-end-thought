<template>
    <panel title='新品推荐' :class='$style.panel'>
        <!--不是用类定义样式的，使用子选择器-->
        <section :class='$style.content'>
            <div class='arrow'>更多尖货</div>
            <slider :options='options' :items='items' cname='product-slider'></slider>
        </section>
    </panel>
</template>

<script>
  import Slider from '../core/slider'
  import Panel from '../core/panel.vue'

  export default {
    components: {
      Slider,
      Panel
    },
    data() {
      return {
        items: [{
          href: 'home',
          src: '//img12.360buyimg.com/jrpmobile/jfs/t13963/267/2355123229/48850/254f797a/5a3c59aeN9cb550f6.jpg?width=335&height=421',
        }, {
          href: 'home',
          src: '//img12.360buyimg.com/jrpmobile/jfs/t13021/306/1996997425/21953/bda69db3/5a2f6a17N9da099b1.jpg?width=335&height=421',
        }, {
          href: 'home',
          src: '//img12.360buyimg.com/jrpmobile/jfs/t14125/310/1997192193/46667/3c910f8b/5a2f6a36Nad95b650.jpg?width=335&height=421',
        }, {
          href: 'home',
          src: '//img12.360buyimg.com/jrpmobile/jfs/t15784/188/381232069/39444/8878571d/5a2f6a4aNbd5a574c.jpg?width=335&height=421',
        }],
        options: {
          slidesPerView: 2.3,
          spaceBetween: 30,
          freeMode: true
        }
      }
    }
  }
</script>

<style lang="scss">
    .product-slider{
        .swiper-container{
            box-sizing: border-box;
            padding: 0 24px;
            .swiper-slide{
                a{
                    display: inline-block;
                    width: 100%;
                    img{
                        width: 100%;
                        display: block;
                        height: 314px;
                        border: 1px solid #fafafa;
                    }
                }
            }
        }
    }
</style>

<style lang="scss" module>
    @import "../../css/element.scss";
    .panel{
        @include panel;
        .content{
            padding-bottom: 40px;
            position: relative;

            &>div:first-child{
                position: absolute;
                font-size: 28px;
                color: #999;
                right:20px;
                top: -70px;
            }
        }
    }
</style>
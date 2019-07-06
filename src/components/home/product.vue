<template>
  <panel :title="title">
    <slider :items="items" :swiperOption="swiperOption" :cname="product-slider"></slider>
    <div class="space"></div>
  </panel>
</template>
<script>
import panel from '_c/core/panel.vue'
import slider from '_c/core/slider.vue'
export default {
  components: {
    panel,
    slider
  },
  props: {
    title: {
      type: String,
      default: ''
    },
    items: {
      type: Array,
      default: () => []
    },
    swiperOption: {
      type: Object,
      default () {
        return {
          slidesPerView: 2.9,
          spaceBetween: 10,
          freeMode: true
        }
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
<style lang="scss" scoped>
.space {
  width: 100%;
  height: 60px;
}
</style>

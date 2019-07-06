<template>
  <section :class="cname">
    <swiper class="swiper-box" :options="swiperOption">
      <swiper-slide class="swiper-item" v-for="(item, index) in items" :key="index">
        <router-link :to="{ name: item.href}">
          <img class="img" :src="item.src" />
        </router-link>
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </section>
</template>

<script>
import 'swiper/dist/css/swiper.css'
import { swiper, swiperSlide } from 'vue-awesome-swiper'
export default {
  components: {
    swiper,
    swiperSlide
  },
  props: {
    cname: {
      type: String,
      default: ''
    },
    items: {
      type: Array,
      default () {
        return []
      }
    },
    swiperOption: {
      type: Object,
      default () {
        return {
          autoplay: true,
          loop: true,
          pagination: {
            el: '.swiper-pagination'
          },
          notNextTick: false
        }
      }
    }
  }
}
</script>
<style lang="scss">
.swiper-box {
  .swiper-item {
    height: 100%;
    &>a>.img {
      width: 100%;
      height: auto;
    }
  }
}
</style>

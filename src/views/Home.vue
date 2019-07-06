<template>
  <div class="home">
    <m-header :title="title"></m-header>
    <h-slider />
    <novice />
    <product v-for="(pro, index) in products" :key="index" :title="pro.title" :items="pro.imgs" />
    <navbar :navlinks="navlinks" />
  </div>
</template>

<script>
import mHeader from '_c/public/header.vue'
import hSlider from '_c/home/hSlider.vue'
import novice from '_c/home/novice.vue'
import product from '_c/home/product.vue'
import navbar from '_c/public/navbar.vue'
export default {
  components: {
    mHeader,
    hSlider,
    novice,
    product,
    navbar
  },
  data () {
    return {
      title: '京东金融',
      products: [
        {
          title: '赏金任务',
          imgs: [
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26893/316/1416172900/5740/58f20b1e/5bc82e3aN7aa90a89.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26767/72/1365822552/8516/2e071d95/5bc82e6eN0be93809.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26893/316/1416172900/5740/58f20b1e/5bc82e3aN7aa90a89.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26767/72/1365822552/8516/2e071d95/5bc82e6eN0be93809.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26893/316/1416172900/5740/58f20b1e/5bc82e3aN7aa90a89.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26767/72/1365822552/8516/2e071d95/5bc82e6eN0be93809.png?width=210&height=260'
            }
          ]
        },
        {
          title: '赏金任务',
          imgs: [
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26893/316/1416172900/5740/58f20b1e/5bc82e3aN7aa90a89.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26767/72/1365822552/8516/2e071d95/5bc82e6eN0be93809.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26893/316/1416172900/5740/58f20b1e/5bc82e3aN7aa90a89.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26767/72/1365822552/8516/2e071d95/5bc82e6eN0be93809.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26893/316/1416172900/5740/58f20b1e/5bc82e3aN7aa90a89.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26767/72/1365822552/8516/2e071d95/5bc82e6eN0be93809.png?width=210&height=260'
            }
          ]
        },
        {
          title: '赏金任务',
          imgs: [
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26893/316/1416172900/5740/58f20b1e/5bc82e3aN7aa90a89.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26767/72/1365822552/8516/2e071d95/5bc82e6eN0be93809.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26893/316/1416172900/5740/58f20b1e/5bc82e3aN7aa90a89.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26767/72/1365822552/8516/2e071d95/5bc82e6eN0be93809.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26893/316/1416172900/5740/58f20b1e/5bc82e3aN7aa90a89.png?width=210&height=260'
            },
            {
              href: 'home',
              src:
                'https://img12.360buyimg.com/jrpmobile/jfs/t26767/72/1365822552/8516/2e071d95/5bc82e6eN0be93809.png?width=210&height=260'
            }
          ]
        }
      ],
      navlinks: [
        {
          name: 'home',
          src:
            'https://img12.360buyimg.com/jrpmobile/jfs/t1/931/18/14488/935/5bda58fdE542c2cc7/f29a349a4ed750ca.png?width=60&height=60'
        },
        {
          name: 'money',
          src:
            'https://img12.360buyimg.com/jrpmobile/jfs/t1/931/18/14488/935/5bda58fdE542c2cc7/f29a349a4ed750ca.png?width=60&height=60'
        }
      ]
    }
  }
}
</script>
<style lang="scss" scoped>
.home {
  padding-bottom: 100px;
}
</style>

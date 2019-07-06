<template>
  <div class="content">
    <c-slider :items="items"></c-slider>
    <section class="menu">
      <div class="item" v-for="(item,index) in enters" :key="index">
        <router-link :to="{name: item.href}">
          <img :src="item.img" />
          <h4>{{item.title}}</h4>
        </router-link>
      </div>
    </section>
  </div>
</template>
<script>
import cSlider from '_c/core/slider.vue'
export default {
  components: {
    cSlider
  },
  data () {
    return {
      items: [
        {
          href: 'home',
          src:
            'https://img12.360buyimg.com/jrpmobile/jfs/t1/52802/14/4027/212241/5d1b14f4Ed1748086/588363d90a40b28c.png?width=750&height=320'
        },
        {
          href: 'home',
          src:
            'https://img12.360buyimg.com/jrpmobile/jfs/t1/54124/12/3394/140400/5d11e389Ee12d74f3/f3cba452b6470938.png?width=750&height=320'
        }
      ],
      enters: [
        {
          href: 'download',
          img:
            'https://img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132',
          title: '优惠券'
        },
        {
          href: 'home',
          img:
            'https://img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132',
          title: '领红包'
        },
        {
          href: 'home',
          img:
            'https://img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132',
          title: '抢钢镚'
        },
        {
          href: 'home',
          img:
            'https://img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132',
          title: '领京豆'
        },
        {
          href: 'home',
          img:
            '//img12.360buyimg.com/jrpmobile/jfs/t5488/298/1036263348/12073/b4f4de97/590ac8e8Ne9def22e.png?width=135&height=135',
          title: '白条提额'
        },
        {
          href: 'download',
          img:
            'https://img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132',
          title: '优惠券'
        },
        {
          href: 'home',
          img:
            'https://img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132',
          title: '领红包'
        },
        {
          href: 'home',
          img:
            'https://img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132',
          title: '抢钢镚'
        },
        {
          href: 'home',
          img:
            'https://img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132',
          title: '领京豆'
        },
        {
          href: 'home',
          img:
            '//img12.360buyimg.com/jrpmobile/jfs/t5488/298/1036263348/12073/b4f4de97/590ac8e8Ne9def22e.png?width=135&height=135',
          title: '白条提额'
        }
      ]
    }
  }
}
</script>
<style lang="scss" scoped>
.content {
  padding-top: 90px;
  .menu {
    display: flex;
    background: #fff;
    padding-bottom: 20px;
    flex-wrap: wrap;
    .item {
      text-align: center;
      width: 20%;
      margin: 40px 0;
      img {
        width: 90px;
        height: 90px;
      }
      h4 {
        font-size: 26px;
        margin-top: 12px;
        color: #666;
        text-align: center;
      }
    }
  }
}
</style>

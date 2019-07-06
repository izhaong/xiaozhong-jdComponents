<template>
  <div class="navbar">
    <ul class="content">
      <li v-for="(item, index) in navlinks" :key="index">
        <router-link :to="{name: item.name}">
          <img
            :src="item.src"
            alt
          />
          <p>首页</p>
        </router-link>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  props: {
    navlinks: {
      type: Array,
      default: () => []
    }
  }
}
</script>
<style lang="scss" scoped>
.navbar {
  width: 100%;
  height: 100px;
  background: #fff;
  position: fixed;
  bottom: 0;
  left: 0;
  z-index: 9999;
  .content {
    display: flex;
    li {
      flex: 1;
      text-align: center;
      a {
        img {
          width: 44px;
          height: 44px;
          margin: 12px auto 6px;
        }
        p {
          font-size: 22px;
          color: #656565;
        }
      }
      .router-link-exact-active {
        p {
          color: #508CEE;
        }
      }
    }
  }
}
</style>

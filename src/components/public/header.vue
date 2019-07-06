<template>
  <div class="header">
    <div class="left">
      <i class="iconfont icon-xiangzuo"></i>
    </div>
    <div class="title">{{title}}</div>
    <div class="right">
      <i class="iconfont icon-caidan"></i>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: ''
    }
  }
}
</script>
<style lang="scss" scoped>
.header {
  display: flex;
  font-family: "PingHei", "Lucida Grande", "Lucida Sans Unicode", "STHeiti",
    "Helvetica", "Arial", "Verdana", "sans-serif";
  font-size: 32px;
  color: #252525;
  width: 100%;
  min-height: 88px;
  border-bottom: 1px solid #e5e5e5;
  background: #fff;
  position: fixed;
  z-index: 9999;
  .left {
    position: relative;
    width: 80px;
    height: 88px;
    i {
      margin: 24px 0 0 20px;
      width: 100%;
      color: #333;
      height: 100%;
      line-height: 88px;
    }
  }
  .title {
    flex: 1;
    line-height: 88px;
    text-align: center;
    color: #333;
    text-overflow: ellipsis;
    white-space: nowrap;
  }
  .right {
    width: 80px;
    height: 100%;
    i {
      margin: 24px 0 0 20px;
      color: #333;
      width: 100%;
      height: 100%;
      line-height: 88px;
    }
  }
}
</style>

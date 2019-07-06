<template>
  <pannel :title="title">
    <section class="content">
      <div class="item" v-for="(item, index) in items" :key="index">
        <div class="head">
          <span class="text">{{item.title}}</span>&nbsp;
          <span class="mark">&nbsp;{{item.mark}}&nbsp;</span>
        </div>
        <div class="value">{{item.value}}%</div>
        <p class="desc">{{item.desc}}</p>
      </div>
    </section>
  </pannel>
</template>
<script>
import pannel from '_c/core/panel.vue'
export default {
  components: {
    pannel
  },
  data () {
    return {
      title: '新手特权',
      items: [
        {
          title: '长乐盈',
          mark: '180天可抵压',
          value: 5.8,
          desc: '近一年历史年华投资回报率'
        },
        {
          title: '长乐盈',
          mark: '180天可抵压',
          value: 5.8,
          desc: '近一年历史年华投资回报率'
        },
        {
          title: '长乐盈',
          mark: '180天可抵压',
          value: 5.8,
          desc: '近一年历史年华投资回报率'
        },
        {
          title: '长乐盈',
          mark: '180天可抵压',
          value: 5.8,
          desc: '近一年历史年华投资回报率'
        }
      ]
    }
  }
}
</script>
<style lang="scss" scoped>
.content {
  display: flex;
  flex-wrap: wrap;
  .item {
    width: 50%;
    padding-left: 32px;
    height: 220px;
    box-sizing: border-box;
    .head {
      color: #333;
      height: 42px;
      line-height: 42px;
      box-sizing: border-box;
      margin: 34px 0 16px;
      white-space: nowrap;
      text-overflow: ellipsis;
      overflow: hidden;
      .text {
        color: #333;
        font-weight: 700;
        font-size: 30px;
      }
      .mark {
        color: #ff5155;
        box-sizing: border-box;
        border: 1px solid #ff5155;
      }
    }
    .value {
      font-weight: 700;
      font-size: 44px;
      height: 58px;
      line-height: 58px;
      color: #ff5155;
      white-space: nowrap;
      text-overflow: ellipsis;
      overflow: hidden;
    }
    .desc {
      font-size: 24px;
      height: 34px;
      line-height: 34px;
      color: #999;
      white-space: nowrap;
      text-overflow: ellipsis;
      overflow: hidden;
    }
  }
}
</style>

<template>
<div>
  <div class="title">热销推荐</div>
  <ul>
    <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
      <img class="item-img" :src="item.imgUrl" alt="">
      <div class="item-info">
        <p class="item-title">{{item.title}}</p>
        <p class="item-desc">{{item.desc}}</p>
        <button class="item-button">查看详情</button>
      </div>
    </li>
  </ul>
</div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl:'http://img1.qunarzz.com/sight/p0/1505/18/18ffcca94b1b7ca2.water.jpg_200x200_9b0d2dc4.jpg',
        title: '长恨歌',
        desc: '多彩贵州城极地海洋世界',
      },
      {
        id: '0002',
        imgUrl:'http://img1.qunarzz.com/sight/p0/1505/18/18ffcca94b1b7ca2.water.jpg_200x200_9b0d2dc4.jpg',
        title: '长恨歌',
        desc: '多彩贵州城极地海洋世界',
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title {
    margin-top .2rem
    line-height: .8rem
    background: #eee
    text-indent: .2rem
  }
  .item {
    overflow: hidden
    display: flex
    height: 1.9rem
    .item-img {
      width: 1.7rem
      height: 1.7rem
      padding: .1rem
    }
    .item-info {
      flex: 1
      padding: .1rem
      min-width: 0
      .item-title {
        line-height: .54rem
        font-size: .32rem
        ellipsis()
      }
      .item-desc {
        line-height .4rem
        color: #ccc
        ellipsis()
      }
      .item-button {
        line-height: .44rem
        margin-top: .16rem
        background: #ff9300
        padding: 0 .2rem
        border-radius: .06rem
        color: #fff
        ellipsis()

      }
    }
  }
</style>
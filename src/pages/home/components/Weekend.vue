<template>
<div>
  <div class="title">周末去哪儿</div>
  <ul>
    <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
      <div class="item-img-wrapper">
        <img class="item-img" :src="item.imgUrl" alt="">
      </div>
      <div class="item-info">
        <p class="item-title">{{item.title}}</p>
        <p class="item-desc">{{item.desc}}</p>
      </div>
    </li>
  </ul>
</div>
</template>

<script>
export default {
  name: 'HomeWeekend',
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
  .item-img-wrapper {
    overflow: hidden
    height: 0
    padding-bottom: 33.9%
    .item-img {
      width: 100%
    }
  }
  .item-info {
    padding: .1rem
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
  }
  
</style>
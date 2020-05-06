<template>
  <div class="header">
    <home-header></home-header>
    <home-swiper></home-swiper>
    <div>test</div>
  </div>
</template>

<script>
import HomeHeader from "./components/Header"
import HomeSwiper from "./components/Swiper"

export default {
  // import引入的组件需要注入到对象中才能使用
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwiper
  }
};
</script>

<style lang='stylus' scoped>
</style>

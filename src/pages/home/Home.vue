<template>
  <div class="header">
    <home-header></home-header>
  </div>
</template>

<script>
import HomeHeader from "./components/Header"
export default {
  // import引入的组件需要注入到对象中才能使用
  name: 'Home',
  components: {
    HomeHeader
  }
};
</script>

<style lang='stylus' scoped>
</style>

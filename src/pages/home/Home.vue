<template>
  <div>
    <!--对应HomeHeader组件，vue会大小写自动关联-->
       <home-header></home-header>
       <home-swiper></home-swiper>
  </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
export default {
  name: 'Home',
  components: {HomeSwiper, HomeHeader},
  comments: {
    HomeHeader: HomeHeader,
    HomeSwiper: HomeSwiper
  }
}
</script>

<style>
</style>

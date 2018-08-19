<template>
  <div>
    <!--对应HomeHeader组件，vue会大小写自动关联-->
       <home-header></home-header>
       <home-swiper></home-swiper>
       <home-icons></home-icons>
  </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
import HomeIcons from './components/Icons'
export default {
  name: 'Home',
  components: {HomeIcons, HomeSwiper, HomeHeader},
  comments: {
    HomeHeader: HomeHeader,
    HomeSwiper: HomeSwiper,
    HomeIcons: HomeIcons
  }
}
</script>

<style>
</style>

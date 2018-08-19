<template>
  <div>
    <!--对应HomeHeader组件，vue会大小写自动关联-->
       <home-header></home-header>
       <home-swiper></home-swiper>
       <home-icons></home-icons>
       <home-recommend></home-recommend>
       <home-weekend></home-weekend>
  </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
import HomeIcons from './components/Icons'
import HomeRecommend from './components/Recommend'
import HomeWeekend from './components/Weekend'
export default {
  name: 'Home',
  components: {HomeWeekend, HomeRecommend, HomeIcons, HomeSwiper, HomeHeader},
  comments: {
    HomeHeader: HomeHeader,
    HomeSwiper: HomeSwiper,
    HomeIcons: HomeIcons,
    HomeRecommend: HomeRecommend,
    HomeWeekend: HomeWeekend
  }
}
</script>

<style>
</style>

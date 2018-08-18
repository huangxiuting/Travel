<template>
  <div>
    <!--对应HomeHeader组件，vue会大小写自动关联-->
       <home-header>

       </home-header>
  </div>
</template>

<script>
import HomeHeader from './components/Header'
export default {
  name: 'Home',
  components: {HomeHeader},
  comments: {
    HomeHeader: HomeHeader
  }
}
</script>

<style>
</style>

<template>
  <div class="search">
    <input type="text" class="search-input" placeholder="输入城市名或拼音"/>
  </div>
</template>

<script>
export default {
  name: 'CitySearch'
}
</script>

<style lang="stylus" scoped>
  @import '~@/assets/styles/varibles.styl'
  .search
    padding : 0.1rem  0.2rem
    height : .72rem
    background : $bgColor
    .search-input
      box-sizing : border-box
      height : .62rem
      line-height : .62rem
      width : 100%
      text-align : center
      border-radius : .06rem
      color : #666
      padding : 0  .1rem
</style>

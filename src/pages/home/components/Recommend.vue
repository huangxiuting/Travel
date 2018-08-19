<template>
  <div>
    <div class="title">
      热销推荐
    </div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl"/>
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
  data: function () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1611/fa/faa1d25b92cec185a3.img.jpg_200x200_435a4fa7.jpg',
        title: '大连圣亚海洋世界',
        desc: '浪漫大连首站，浪漫的海洋主题公园'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/201403/10/664cdc5201921ee8e301956837e8eaec.jpg_200x200_4fa8d902.jpg',
        title: '大连圣亚海洋世界',
        desc: '浪漫大连首站，浪漫的海洋主题公园'
      }, {
        id: '00031',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/201403/10/664cdc5201921ee8e301956837e8eaec.jpg_200x200_4fa8d902.jpg',
        title: '大连圣亚海洋世界',
        desc: '浪漫大连首站，浪漫的海洋主题公园'
      }, {
        id: '0004',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/201403/10/664cdc5201921ee8e301956837e8eaec.jpg_200x200_4fa8d902.jpg',
        title: '大连圣亚海洋世界',
        desc: '浪漫大连首站，浪漫的海洋主题公园'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~@/assets/styles/mixins.styl'
  .title
    margin-top : .2rem
    line-height : .8rem
    background : #eee
    text-indent : .2rem
  .item
    overflow hidden
    display : flex
    height : 1.9rem
    /*background : red*/
    .item-img
      width : 1.7rem
      height : 1.7rem
      padding : .1rem
    .item-info
      flex : 1
      padding : .1rem
      /*...小技巧显示*/
      min-width : 0
      .item-title
        line-height : .54rem
        font-size : .32rem
        ellipsis()
      .item-desc
        line-height : .4rem
        color : #ccc
        ellipsis()
      .item-button
        line-height : .44rem
        margin-top : .16rem
        background : #ff9300
        padding : 0 .2rem
        border-radius : .6rem
        color : #fff
</style>

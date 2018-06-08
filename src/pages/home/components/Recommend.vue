<template>
  <div>
    <div class="recommend-title">热销推荐</div>
    <ul>
      <li class="item" v-for="item of recommendList" :key="item.id">
        <img :src="item.imgUrl" class="item-img">
        <div class="item-info border-bottom">
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
  props: ['recommendList'],
  data: function () {
    return {
      recommendLis: [{
        id: '001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/f4/f455d92ba582f608.water.jpg_200x200_375e5775.jpg',
        title: '海洋馆',
        desc: '浪漫的海洋馆浪漫的海洋馆浪漫的海洋馆浪漫的海洋馆浪漫的海洋馆浪漫的海洋馆'
      }, {
        id: '004',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/f4/f455d92ba582f608.water.jpg_200x200_375e5775.jpg',
        title: '海洋馆',
        desc: '浪漫的海洋馆浪漫的海洋馆浪漫的海洋馆浪漫的海洋馆浪漫的海洋馆浪漫的海洋馆'
      }, {
        id: '003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/f4/f455d92ba582f608.water.jpg_200x200_375e5775.jpg',
        title: '海洋馆',
        desc: '浪漫的海洋馆浪漫的海洋馆浪漫的海洋馆浪漫的海洋馆浪漫的海洋馆浪漫的海洋馆'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .recommend-title
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-indent: .2rem
  .item
    display: flex
    height: 1.9rem
    overflow: hidden
    .item-img
      width: 1.7rem
      height: 1.7rem
      padding: .1rem
    .item-info
      flex: 1
      padding: .1rem
      .item-title
        height: .54rem
        font-size: .32rem
      .item-desc
        color: #ccc
        height: .4rem
      .item-button
        background-color: #ff9300
        line-height: .44rem
        padding: 0 .16rem
        color: #fff
        border-radius: .06rem
</style>

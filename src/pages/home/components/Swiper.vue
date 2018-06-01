<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="item of swiperList" :key="item.id"><img class="swiper-img"  :src="item.imgUrl"></swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script >
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        autoplay: 3000,
        pagination: '.swiper-pagination',
        paginationClickable: true
      },
      swiperList: [{
        id: '01',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1805/77/f63bd04dd5319602.jpg_750x200_6ba8e0ca.jpg'
      },
      {
        id: '02',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1805/e6/33ce6413c5949f02.jpg_750x200_004a9ea4.jpg'
      },
      {
        id: '03',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1806/4a/ba45db469d304d02.jpg_750x200_57d60cca.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wrapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 26.666%
    background-color: #ccc
  .swiper-img
      width: 100%
</style>

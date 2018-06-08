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
  props: ['swiperList'],
  data () {
    return {
      swiperOption: {
        autoplay: 3000,
        pagination: '.swiper-pagination',
        paginationClickable: true
      }
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wrapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 30.666%
    background-color: #ccc
  .swiper-img
      width: 100%
</style>

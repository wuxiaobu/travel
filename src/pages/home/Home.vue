<template>
  <div>
    <home-header></home-header>
    <home-swiper></home-swiper>
    <home-icons></home-icons>
    <home-recommend></home-recommend>
  </div>
</template>

<script>
import HomeHeader from '@/pages/home/components/Header'
import HomeSwiper from '@/pages/home/components/Swiper'
import HomeIcons from '@/pages/home/components/Icons'
import HomeRecommend from '@/pages/home/components/Recommend'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwiper,
    HomeIcons,
    HomeRecommend
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>

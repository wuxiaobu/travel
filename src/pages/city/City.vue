<template>
  <div>
    <city-header></city-header>
    <city-search></city-search>
    <city-list></city-list>
  </div>
</template>

<script>
import CityHeader from '@/pages/city/components/Header'
import CitySearch from '@/pages/city/components/Search'
import CityList from '@/pages/city/components/List'
export default {
  name: 'City',
  components: {
    CityHeader,
    CitySearch,
    CityList
  }
}
</script>

<style lang="stylus" scoped>

</style>

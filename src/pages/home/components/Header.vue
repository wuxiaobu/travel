<template>
  <div class="header">
    <div class="header-letf"><i class="fa fa-chevron-left"></i></div>
    <div class="header-input">输入城市/景点/游玩主题</div>
    <router-link to='/city'>
      <div class="header-right">{{this.city}}<i class="fa fa-caret-down"></i></div>
    </router-link>
  </div>
</template>
<script>
export default {
  name: 'HomeHeader',
  props: ['city']

}
</script>

<style lang="stylus" scoped>
  .header
      display: flex
      line-height: .86rem
      background: #00bcd4
      color: #fff
      .header-left
        width: .84rem
        float: left
        text-align: center
        font-size: .4rem
      .header-input
        flex: 1
        height: .64rem
        line-height: .64rem
        margin-top: .12rem
        margin-left: .2rem
        padding-left: .2rem
        background: #fff
        border-radius: .1rem
        color: #ccc
      .header-right
        min-width: 1.04rem
        padding: 0 .1rem
        float: right
        text-align: center
        color: #fff
</style>

<template>
  <div class="list" ref="wrapper">
    <div>
    <div class="area">
      <div class="title border-topbottom">当前城市</div>
      <div class="button-list">
        <div class="button-wrap">
          <div class="button">南京</div>
        </div>
      </div>
    </div>
    <div class="area">
      <div class="title border-topbottom">热门城市</div>
      <div class="button-list">
        <div class="button-wrap">
          <div class="button">南京</div>
        </div>
        <div class="button-wrap">
          <div class="button">南京</div>
        </div>
        <div class="button-wrap">
          <div class="button">南京</div>
        </div>
        <div class="button-wrap">
          <div class="button">南京</div>
        </div>
        <div class="button-wrap">
          <div class="button">南京</div>
        </div>
      </div>
    </div>
    <div class="area">
      <div class="title border-topbottom">A</div>
      <div class="item-list">
        <div class="item">
          afaf
        </div>
        <div class="item">
          afaf
        </div>
        <div class="item">
          afaf
        </div>
        <div class="item">
          afaf
        </div>
      </div>
      <div class="title border-topbottom">B</div>
      <div class="item-list">
        <div class="item">
          afaf
        </div>
        <div class="item">
          afaf
        </div>
        <div class="item">
          afaf
        </div>
        <div class="item">
          afaf
        </div>
      </div>
      <div class="title border-topbottom">C</div>
      <div class="item-list">
        <div class="item">
          afaf
        </div>
        <div class="item">
          afaf
        </div>
        <div class="item">
          afaf
        </div>
        <div class="item">
          afaf
        </div>
      </div>
    </div>
  </div>
  </div>
</template>

<script>
import BScroll from 'better-scroll'
export default {
  name: 'CityList',
  mounted () {
    this.scroll = new BScroll(this.$refs.wrapper)
  }
}
</script>

<style lang="stylus" scoped>
  .list
    position: absolute
    top: 1.78rem
    left: 0
    right: 0
    bottom: 0
    overflow: hidden
    .title
      line-height: .4rem
      background-color: #eee
      padding-left: .2rem
      color: #666
      font-size: .26rem
    .button-list
      overflow: hidden
      padding: .1rem .6rem .1rem .1rem
      .button-wrap
        float: left
        width: 33.33%
        .button
          margin: .1rem
          padding: .1rem
          text-align: center
          border: .02rem solid #ccc
          border-radius: .06rem
    .item-list
      .item
        line-height: .76rem
        padding-left .2rem
        color: #666
</style>





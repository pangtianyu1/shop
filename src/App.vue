<template>
  <div id="app">
    <router-view></router-view>
    <!-- 路由配置里面默认有个meta空对象  可以设置值为true或者false来控制此组件显不显示的状态 -->
<FooterGuide v-show="$route.meta.showFooter"></FooterGuide>
  </div>
</template>

<script>
import FooterGuide from './components/FooterGuide/FooterGuide'
export default {
  components:{
    FooterGuide
  }
}
</script>

<style lang="stylus" ref="stylesheet/stylus">
  #app
      width 100%
      height 100%
      background-color #fff
</style>

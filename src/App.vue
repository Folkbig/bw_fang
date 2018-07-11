<style lang="stylus" rel="stylesheet/stylus">
  #app
    max-width 414px
    height 100%
    background #f5f5f5
    margin 0 auto
</style>

<template>
  <div id="app">
    <router-view></router-view>
    <FooterGuide v-show="$route.meta.showFooter"></FooterGuide>
  </div>
</template>


<script>
  import FooterGuide from './components/FooterGuide/FooterGuide.vue'

  export default {
    components: {
      FooterGuide
    }
  }
</script>

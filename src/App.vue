<template>
  <div id="app">
    <HeaderDc class="container"/>
    <MainContent />
    <MainContentFooter />
  </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue'
import MainContent from './components/MainContent.vue'
import MainContentFooter from './components/MainContentFooter.vue'

export default {
  name: 'App',
  components: {
    HeaderDc,
    MainContent,
    MainContentFooter
  }
}
</script>

<style lang="scss">
 @import './assets/style/style';
</style>

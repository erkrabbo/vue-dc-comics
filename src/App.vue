<template>
  <div id="app">
    <HeaderDc class="container"/>
    <MainContent />
    <MainContentFooter />
    <AppFooter />
  </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue'
import MainContent from './components/MainContent.vue'
import MainContentFooter from './components/MainContentFooter.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  name: 'App',
  components: {
    HeaderDc,
    MainContent,
    MainContentFooter,
    AppFooter
  }
}
</script>

<style lang="scss">
 @import './assets/style/style';
</style>

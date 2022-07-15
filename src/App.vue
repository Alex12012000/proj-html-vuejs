<template>
  <div id="app">
    <!-- Header con props per voci menu -->
    <PageHeader :headerMenu="headMenu"/>
    <!-- Main con relative section -->
    <main>
      <PageJumbotron/>
      <MarketingCards/>
      <MainFeatures/>
    </main>
    <!-- Footer con props per voci menu -->
  </div>
</template>

<script>
// import MainFeatures from './components/MainFeatures.vue'
import PageHeader from './components/PageHeader.vue'
import PageJumbotron from './components/PageJumbotron.vue'
import MarketingCards from './components/MarketingCards.vue'
import MainFeatures from './components/MainFeatures.vue'

export default {
  name: 'App',
  components: {
    PageHeader,
    PageJumbotron,
    MarketingCards,
    MainFeatures

  },
  data() {
    return {
      headMenu: ['Home', 'About us', 'Feature', 'Testimonials', 'Contact US']
    }
  },
}
</script>

<style lang="scss">
@import './style/common.scss';
</style>

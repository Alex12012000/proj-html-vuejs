<template>
  <div id="app">
    <!-- Header con props per voci menu -->
    <PageHeader :headerMenu="headMenu"/>
    <!-- Main con relative section -->
    <main>
      <PageJumbotron/>
      <MarketingCards/>
      <MainFeatures/>
      <PopularFeatures/>
      <TestimonialSection/>
      <LastPosts/>
    </main>
    <!-- Footer con props per voci menu -->
  </div>
</template>

<script>
// import LastPosts from './components/LastPosts.vue'
import PageHeader from './components/PageHeader.vue'
import PageJumbotron from './components/PageJumbotron.vue'
import MarketingCards from './components/MarketingCards.vue'
import MainFeatures from './components/MainFeatures.vue'
import PopularFeatures from './components/PopularFeatures.vue'
import TestimonialSection from './components/TestimonialSection.vue'
import LastPosts from './components/LastPosts.vue'

export default {
  name: 'App',
  components: {
    PageHeader,
    PageJumbotron,
    MarketingCards,
    MainFeatures,
    PopularFeatures,
    TestimonialSection,
    LastPosts

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

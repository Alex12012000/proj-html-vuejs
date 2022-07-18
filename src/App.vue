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
      <MapAndForm/>
    </main>

    <!-- Footer con props per voci menu -->
    <PageFooter :menuLinks="menuFooterLink" :aboutLinks="aboutUsLink"/>
    
  </div>
</template>

<script>
// import PageFooter from './components/PageFooter.vue'
import PageHeader from './components/PageHeader.vue'
import PageJumbotron from './components/PageJumbotron.vue'
import MarketingCards from './components/MarketingCards.vue'
import MainFeatures from './components/MainFeatures.vue'
import PopularFeatures from './components/PopularFeatures.vue'
import TestimonialSection from './components/TestimonialSection.vue'
import LastPosts from './components/LastPosts.vue'
import MapAndForm from './components/MapAndForm.vue'
import PageFooter from './components/PageFooter.vue'

export default {
  name: 'App',
  components: {
    PageHeader,
    PageJumbotron,
    MarketingCards,
    MainFeatures,
    PopularFeatures,
    TestimonialSection,
    LastPosts,
    MapAndForm,
    PageFooter

  },
  data() {
    return {
      headMenu: ['Home', 'About us', 'Feature', 'Testimonials', 'Contact US'],
      menuFooterLink: ['About Us', 'Theme', 'Features', 'Pricing', 'Blog'],
      aboutUsLink: ['About Sofbox', 'Roadmap', 'How it Work', 'Team', 'News']
    }
  },
}
</script>

<style lang="scss">
@import './style/common.scss';
</style>

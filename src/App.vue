<template>
  <div id="app">
    <!-- Header con props per voci menu -->
    <PageHeader :headerMenu="headMenu"/>
    <!-- Main con relative section -->
    <main>
      <PageJumbotron/>
    </main>
    <!-- Footer con props per voci menu -->
  </div>
</template>

<script>
// import PageJumbotron from './components/PageJumbotron.vue'
import PageHeader from './components/PageHeader.vue'
import PageJumbotron from './components/PageJumbotron.vue'

export default {
  name: 'App',
  components: {
    PageHeader,
    PageJumbotron

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

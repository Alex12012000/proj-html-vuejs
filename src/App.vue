<template>
  <div id="app">
    <!-- Header con props per voci menu -->
    <PageHeader :headerMenu="headMenu"/>
    <!-- Main con relative section -->
    <!-- Footer con props per voci menu -->
  </div>
</template>

<script>
// import PageHeader from './components/PageHeader.vue'
import PageHeader from './components/PageHeader.vue'

export default {
  name: 'App',
  components: {
    PageHeader
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

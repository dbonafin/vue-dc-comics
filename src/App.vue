<template>
  <div id="app">

    <!-- Header content -->
    <header>
      <PageHeader/>
    </header>

    <main>
      <!-- Top section of the main area - Jumbotron -->
      <TopSection/>

      <!-- Comics section - Main section of the page -->
      <ComicsSection/>

      <!-- Shop section - merchandising, subscription etc -->
      <ShopSection/>
    </main>

    <!-- Footer content -->
    <footer>
      <PageFooter/>
    </footer>

  </div>
</template>

<script>

  // Import all the components of the page
  import PageHeader from './components/PageHeader.vue';
  import TopSection from './components/TopSection.vue';
  import ComicsSection from './components/ComicsSection.vue'
  import ShopSection from './components/ShopSection.vue';
  import PageFooter from './components/PageFooter.vue';
  

  export default {
    name: 'App',
    components: {
      PageHeader,
      TopSection,
      ComicsSection,
      ShopSection,
      PageFooter
    }
  }

</script>

<style lang="scss">

  @import "./style/common.scss";

</style>

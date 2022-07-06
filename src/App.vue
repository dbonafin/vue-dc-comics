<template>
  <div id="app">

    <!-- Header content -->
    <header>
      <PageHeader/>
    </header>

    <main>
      <!-- Top section of the main area -->
      <TopSection/>

      <!-- Shop section - merchandising, subscription etc -->
      <ShopSection/>
    </main>
 
  </div>
</template>

<script>

  // Import all the components of the page
  import PageHeader from './components/PageHeader.vue';
  import TopSection from './components/TopSection.vue';
  import ShopSection from './components/ShopSection.vue';

  export default {
    name: 'App',
    components: {
      PageHeader,
      TopSection,
      ShopSection
    }
  }

</script>

<style lang="scss">

  @import "./style/common.scss";

</style>

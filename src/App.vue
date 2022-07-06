<template>
  <div id="app">

    <!-- Header content -->
    <header>
      <PageHeader/>
    </header>

    <main>
      <!-- Top section of the main area -->
      <TopSection/>

    </main>
 
  </div>
</template>

<script>
import PageHeader from './components/PageHeader.vue';
import TopSection from './components/TopSection.vue';


export default {
  name: 'App',
  components: {
    PageHeader,
    TopSection,
}
}
</script>

<style lang="scss">
@import "./style/common.scss";

</style>

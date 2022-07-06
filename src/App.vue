<template>
  <div id="app">

    <header>
      <PageHeader/>
    </header>
 
  </div>
</template>

<script>
import PageHeader from './components/PageHeader.vue';"./components/PageHeader.vue";

export default {
  name: 'App',
  components: {
    PageHeader
  }
}
</script>

<style lang="scss">
@import "./style/common.scss";

header {
  background-color: white;
}
</style>

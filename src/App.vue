<template>
  <div>
    <Navigation></Navigation>
    <GitChart></GitChart>
  </div>
</template>

<script>
  import Navigation from './components/Navigation.vue';
  import GitChart from './components/GitChart.vue';
  export default {
    components: {
      Navigation,
      GitChart
    }
  }
</script>

<style lang="scss">
  @import '../node_modules/bulma/bulma.sass';
</style>

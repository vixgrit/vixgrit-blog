<template lang="html">
  <div class="columns is-desktop">
    <div class="column is-12">
      <a :href="githubLink">
        <img class="githubChart" :src="githubChart" />
      </a>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      githubLink: 'https://github.com/vixgrit',
      githubChart: 'http://ghchart.rshah.org/vixgrit'
    }
  }
}
</script>

<style lang="css">
  .githubChart {
    display:block;
    margin: auto;
    width: 90%
  }
</style>

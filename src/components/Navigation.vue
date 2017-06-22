<template lang="html">
  <nav class="nav">
  <div class="nav-left">
    <a class="nav-item">
      <h1 class="title is-4">@vixgrit</h1>
    </a>
    <a class="nav-item" href="https://github.com/vixgrit">
      <span class="icon">
        <i class="fa fa-github"></i>
      </span>
    </a>
    <a class="nav-item" href="https://twitter.com/vixgrit">
      <span class="icon">
        <i class="fa fa-twitter"></i>
      </span>
    </a>
  </div>
  <!-- This "nav-toggle" hamburger menu is only visible on mobile -->
  <!-- You need JavaScript to toggle the "is-active" class on "nav-menu" -->
  <span class="nav-toggle" :class="{'is-active': isActive}" @click="toggleIsActive">
    <span></span>
    <span></span>
    <span></span>
  </span>
  <!-- This "nav-menu" is hidden on mobile -->
  <!-- Add the modifier "is-active" to display it on mobile -->
  <div class="nav-right nav-menu" :class="{'is-active': isActive}">
    <a class="nav-item">
      Home
    </a>
    <a class="nav-item">
      About
    </a>
    <a class="nav-item">
      Blog
    </a>
    <a class="nav-item">
      Projects
    </a>
    <a class="nav-item">
      Contact
    </a>
  </div>
</nav>
</template>

<script>
export default {
  data() {
    return {
      isActive: false
    }
  },
  methods: {
    toggleIsActive() {
      this.isActive = !this.isActive;
    }
  }
}
</script>

<style lang="css">
</style>

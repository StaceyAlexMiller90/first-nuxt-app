<template>
  <div>
    <TheHeader @sidenavToggle="displaySideNav = !displaySideNav" />
    <TheSidenav :show="displaySideNav" @close="displaySideNav = false" />
    <nuxt />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import TheHeader from '@/components/Navigation/TheHeader.vue'
import TheSidenav from '@/components/Navigation/TheSidenav.vue'

export default Vue.extend({
  components: {
    TheHeader,
    TheSidenav,
  },
  data() {
    return {
      displaySideNav: false,
    }
  },
})
</script>

<style>
html {
  font-family: 'Noto Sans', sans-serif;
}

body {
  margin: 0;
}
</style>

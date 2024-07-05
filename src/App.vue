<script >
import AppNav from './components/AppNav.vue'
import AppContent from './components/AppContent.vue'

export default {
  name: 'App',
  components: {
    AppNav,
    AppContent
  }
}
</script>

<template>
  
  <AppNav />
  <AppContent />
</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;

h1,
h2,
h3,
h4,
h5,
h6 {
  color: $primary;
}
</style>

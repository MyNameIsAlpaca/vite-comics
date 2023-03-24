<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppNavbar from './components/AppNavbar.vue'

export default {
  data() {
    return{

    }
  },
  components: {
    AppHeader,
    AppMain,
    AppNavbar,
  }
}
</script>

<template>
  <div class="main-container">
    <AppHeader></AppHeader>
    <AppMain></AppMain>
    <AppNavbar></AppNavbar>
  </div>
</template>

<style scoped>
</style>

<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppNavbar from './components/AppNavbar.vue'
import AppTopFooter from './components/AppTopFooter.vue'

export default {
  data() {
    return{

    }
  },
  components: {
    AppHeader,
    AppMain,
    AppNavbar,
    AppTopFooter,
  }
}
</script>

<template>
  <div class="main-container">
    <AppHeader></AppHeader>
    <AppMain></AppMain>
    <AppNavbar></AppNavbar>
    <AppTopFooter></AppTopFooter>
  </div>
</template>

<style scoped>
</style>

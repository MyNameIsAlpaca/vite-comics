<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppNavbar from './components/AppNavbar.vue'
import AppTopFooter from './components/AppTopFooter.vue'
import AppBottomFooter from './components/AppBottomFooter.vue'

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
    AppBottomFooter,
  }
}
</script>

<template>
  <div class="main-container">
    <AppHeader></AppHeader>
    <AppMain></AppMain>
    <AppNavbar></AppNavbar>
    <AppTopFooter></AppTopFooter>
    <AppBottomFooter></AppBottomFooter>
  </div>
</template>

<style scoped>
</style>

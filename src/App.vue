<template>
  <AppHeader></AppHeader>
  <!-- <div class="container"> -->
    <h1>ここはApp.Vue</h1>
    <AppSecond></AppSecond>
    <AppThird></AppThird>
  <!-- </div> -->
  <AppFooter></AppFooter>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter
  }
}
</script>

<script setup lang="ts">

</script>

<style>
#app {
  background-color: beige;
}
</style>

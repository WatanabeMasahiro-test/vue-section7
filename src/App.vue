<template>
  <AppHeader></AppHeader>
  <!-- <div class="container"> -->
    <h1>ここはApp.Vue</h1>
    <p>{{ msg_f(msg) }}</p>
    <AppSecond :ten-num="tenNum" :fifty-Num="fiftyNum" v-on:my-click="msg_f"></AppSecond>
    <AppThird eight-num="8"></AppThird>
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
  },
  data: () => ({
    msg     : 'App.vue MSG',
    tenNum  : 10,
    fiftyNum : 50,
  }),
  methods: {
    msg_f(value) {
      if(value == "子コンポーネント") {
        this.msg = value
      }
      return this.msg;
    },
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

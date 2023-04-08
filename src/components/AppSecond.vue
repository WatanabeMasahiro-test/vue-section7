<template>
    <div>
        <h5>My AppSecond.vue. second...</h5>
        <p>No.【{{ number }}】</p>
        <button @click="increment">+1</button>
    </div>
</template>

<script>
// import ~~
export default {
    name: 'AppSecond',
  data: () => ({
    number : 123,
  }),
  methods: {
    increment() {
      this.number++;
    }
}
}
</script>

<style scoped>
  div {
    border : 1px solid red;
  }
</style>
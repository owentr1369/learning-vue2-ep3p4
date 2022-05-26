<template>
  <div id="app">
    <div v-for="n in 10" :key="n">{{ n }}</div>
  </div>
</template>

<script>
// v-if se remove phan tu di, con v-show se an phan tu di

export default {
  name: "App",
  data() {
    return {};
  },
  methods: {},
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

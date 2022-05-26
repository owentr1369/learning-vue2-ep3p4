<template>
  <div id="app">
    <h1 v-for="(menu, i) in menus" :key="i">{{ menu }} voi id la {{ i }}</h1>
    <div v-for="(menu, index) in menus" :key="index">
      <h3>{{ menu }}</h3>
      <p>{{ index }}</p>
    </div>
  </div>
</template>

<script>
// v-if se remove phan tu di, con v-show se an phan tu di

export default {
  name: "App",
  data() {
    return {
      menus: ["Home", "About", "Blog"],
    };
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

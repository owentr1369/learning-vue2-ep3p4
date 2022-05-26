<template>
  <div id="app">
    <h1 v-for="(menu, i) in menus" :key="i">{{ menu }} voi id la {{ i }}</h1>
    <ul>
      <li v-for="student in students" :key="student">{{ student.name }}</li>
    </ul>
    <ul>
      <li v-for="student in students" :key="student">{{ student.age }}</li>
    </ul>
    <ul>
      <li v-for="student in students" :key="student">{{ student.class }}</li>
    </ul>
    <ul>
      <li v-for="value in students" :key="value">{{ value }}</li>
      <li v-for="student in students" :key="student">
        <div v-for="value in student" :key="value">{{ value }}</div>
      </li>
    </ul>
  </div>
</template>

<script>
// v-if se remove phan tu di, con v-show se an phan tu di

export default {
  name: "App",
  data() {
    return {
      menus: ["Home", "About", "Blog"],
      students: [
        { name: "Jon", age: 30, class: "CNTT" },
        { name: "Steve", age: 32, class: "QTKD" },
        { name: "Elon", age: 31, class: "CDT" },
      ],
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

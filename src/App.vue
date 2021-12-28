<template>
  <div id="app">
    <h2>3D Viewer with Three.js and Vue 2</h2>
    <Viewer/>
  </div>
</template>

<script>
import Viewer from "./components/Viewer.vue";

export default {
  name: "App",
  components: {
    Viewer,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>

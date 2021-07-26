<template>
  <div>Hello {{ name }}</div>
  <div v-html="channel"></div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "Rusiru Meranga",
      channel: "<b>Vue JS Channel</b>",
    };
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
  margin-top: 60px;
}
</style>

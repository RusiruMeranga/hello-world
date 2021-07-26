<template>
  <div>Hello {{ name }}</div>
  <div v-html="channel"></div>
  <h2 v-bind:id="headingId">Heading</h2>
  <h2 v-bind:class="status">Status</h2>
  <h2 v-bind:class="isSoldOut ? 'sold-out' : 'new'">SoldOut? Movie</h2>
  <button v-bind:disabled="isDisabled">Click me</button>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "Rusiru Meranga",
      channel: "<b>Vue JS Channel</b>",
      headingId: "Heading",
      isDisabled: true,
      status: "danger",
      isSoldOut: false,
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

.underline {
  text-decoration: underline;
}

.danger {
  color: red;
}

.new {
  color: rgb(9, 255, 0);
}

.sold-out {
  color: blueviolet;
}
</style>

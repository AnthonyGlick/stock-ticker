<template>
  <div id="sidebar" v-if="isNotLogin">
    <div id="icons">
      <img class="icon" src="https://via.placeholder.com/50">
      <img class="icon" src="https://via.placeholder.com/50">
      <img class="icon" src="https://via.placeholder.com/50">
      <img class="icon" src="https://via.placeholder.com/50">
      <img class="icon" src="https://via.placeholder.com/50">
    </div>
  </div>
</template>

<script>
export default {
  name: "Sidebar",
  computed: {
      isNotLogin() {
          return this.$route.path !== '/login';
      }
  }
};
</script>

<style>
#sidebar {
  position: fixed;
  width: 75px;
  height: 100%;
  background-color: #eee;
}
.icon {
  padding-top: 10px;
}
</style>

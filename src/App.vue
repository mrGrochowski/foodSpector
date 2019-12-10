<template>
  <div id="app" class="app container">
    <Navbar></Navbar>
    <!--Main Content-->
    <main class="main">
      <router-view />
    </main>
  </div>
</template>
<script>
/* eslint-disable */
import Navbar from "./components/Nav/NavBar.vue";

export default {
  components: {
    Navbar
  }
};
</script>

<style lang="scss">
@import "./assets/css/main.scss";

.app {
  height: 100%;
  background-color: #fdfdfdff;
}

.main {
  height: 100%;
}
</style>

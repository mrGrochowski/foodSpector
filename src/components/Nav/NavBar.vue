<template>
  <nav class="nav-bar pt-3 row">
    <div class="col-6">
      <img class="logo" src="../../../design/assets/logo.svg" alt="food spector logo" />
    </div>
    <div class="col-2 ml-auto">
      <img class="hamburger" src="../../assets/icons/hamburger.svg" alt="" />
    </div>
    <!-- <NavItem></NavItem> -->
  </nav>
</template>

<script>
import NavItem from "./NavItem.vue";
export default {
  data() {
    return { active: [false, false, true, false, false] };
  },
  components: {
    NavItem
  },
  methods: {
    toogleActive(i) {
      this.active[i] != this.active[i];
    }
  }
};
</script>

<style lang="scss" scoped>
.nav-bar {
  position: absolute;
  width: 100%;
  z-index: 1;
}

.logo {
  max-height: 30px;
  width: auto;
}
.hamburger {
  max-height: 30px;
  width: auto;
}
</style>

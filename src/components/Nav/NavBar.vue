<template>
  <nav class="nav-bar row">
    <div class="logo col">🍔 FoodSpector</div>
    <NavItem>Cokolwiek</NavItem>
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
</style>

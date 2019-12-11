<template>
  <div class="home">
    <wellcome-jumbo :header="'Koniec z przeterminowanym jedzeniem'"></wellcome-jumbo>
  </div>
</template>

<script>
// @ is an alias to /src
import WellcomeJumbo from "./WellcomeJumbo.vue";
export default {
  name: "home",
  components: {
    WellcomeJumbo
  }
};
</script>
<style lang="scss" scoped>
.home {
  height: 100%;
}
</style>

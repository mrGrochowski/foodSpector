<template>
  <div class="home">
    <wellcome-jumbo />
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

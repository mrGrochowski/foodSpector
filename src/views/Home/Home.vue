<template>
  <div class="home">
    <wellcome-jumbo />
  </div>
</template>
 
<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import WellcomeJumbo from "./WellcomeJumbo.vue";
export default {
  name: "home",
  components: {
    HelloWorld,
    WellcomeJumbo
  }
};
</script>

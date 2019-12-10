<template>
  <div class="col">
    <slot>
      <span>{{label}}</span>
    </slot>
  </div>
</template>

<script >
export default {
  props: {
    url: {},
    label: {},
    active: {
      default: false
    }
  },
  computed: {
    shuldContenerVisibleAsActive() {
      return this.active
        ? "text-white no-underline hover:text-white"
        : "no-underline hover:text-pink-500";
    },
    shuldLabelVisibleAsAvtive() {
      return this.active
        ? "text-gray-600 md:text-gray-400 block md:inline-block"
        : "text-white md:font-bold block md:inline-block";
    }
  }
};
</script>
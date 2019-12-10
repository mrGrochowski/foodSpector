<template>
  <div class="row">
    <div class="wellcome-jumbo"></div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.wellcome-jumbo {
  display: inline-block;
  width: 100%;
  min-height: 39vh;
  background-color: #fff;
  background-image: url("../../assets/images/laura-mitulla-52-C-unsplash.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  mask-image: linear-gradient(
    180deg,
    rgba(0, 0, 0, 1) 20%,
    rgba(0, 0, 0, 1) 80%,
    rgba(0, 0, 0, 0) 95%
  );
  mask-repeat: space;
}
</style>

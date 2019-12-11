<template>
  <div class="row">
    <div class="wellcome-jumbo col">
      <slot name="header"
        ><h1 v-if="header" class="wellcome-jumbo__header">{{ header }}</h1></slot
      >
      <slot name="description">
        <span class="wellcome-jumbo__description">Kup produkty, a ja zajmę się datą ważności.</span>
      </slot>
    </div>
  </div>
</template>

<script>
export default {
  props: ["header"]
};
</script>

<style lang="scss" scoped>
.wellcome-jumbo {
  display: inline-flex;
  flex-direction: column;
  width: 100%;
  //min-height: 42vh;
  //min-height: 325px;
  background-color: #fff;
  position: relative;
  z-index: 0;
  &:before {
    content: "";
    // position: absolute;
    // left: 0;
    // top: 0;
    // right: 0;
    // bottom: 0px;

    height: 220px;
    margin-left: -15px;
    margin-right: -15px;
    background-image: url("../../assets/images/laura-mitulla-52-C-unsplash.jpg");
    background-repeat: no-repeat;
    background-position: 20%;
    background-size: cover;
    mask-image: linear-gradient(
      180deg,
      rgba(0, 0, 0, 1) 20%,
      rgba(0, 0, 0, 1) 70%,
      rgba(0, 0, 0, 0) 100%
    );
    mask-repeat: space;
    z-index: 0;
  }
}
.wellcome-jumbo__header {
  font-weight: 700;
  line-height: 1.275;
  //justify-self: flex-end;
  z-index: 1;
  color: #4f4f4f;
  font-size: 18px;
  margin-top: -30px;
}

.wellcome-jumbo__description {
  font-weight: 500;
  font-size: 14px;
  padding-top: 10px;

  color: #646464;
}
</style>

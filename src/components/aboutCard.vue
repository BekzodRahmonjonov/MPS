<template>
  <div class="about-card">
    <img :src="img" alt="" />
    <h5 class="heading_sm">{{ heading }}</h5>
    <p class="paragraph">{{ paragraph }}</p>
  </div>
</template>

<script>
export default {
  props: ["heading", "paragraph", "img"],
};
</script>

<style lang="scss">
.about-card {
  border: 1px solid #e6edf5;
  border-radius: 8px;
  width: 270px;
  padding: 32px;
  .heading_sm {
    font-family: "Hind Siliguri";
    font-weight: bold;
    font-size: 24px;
    line-height: 32px;
    color: #333333;
    margin-top: 90px;
  }
  .paragraph {
    font-family: "Work Sans";
    font-size: 16px;
    line-height: 32px;
    color: rgba(51, 51, 51, 0.496405);
    margin-top: 18px;
  }
}
</style>

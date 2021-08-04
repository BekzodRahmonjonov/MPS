<template>
  <div class="part">
    <div class="part__item">
      <img class="part__img" :src="img" />
      <div class="part__number-img">
        <span> {{ number }} </span>
      </div>
    </div>
    <h4 class="heading_sm">{{ heading }}</h4>
    <p class="paragraph">{{ paragraph }}</p>
  </div>
</template>

<script>
export default {
  name: "PortfolioCard",
  props: ["heading", "img", "number", "paragraph"],
};
</script>

<style lang="scss">
.part {
  text-align: center;
  span {
    background: #4db282;
    border-radius: 0px 24px 0px 8px;
    width: 96px;
    height: 96px;
    position: absolute;
    bottom: 0;
    left: 0;
    font-family: "Hind Siliguri";
    font-weight: bold;
    font-size: 40px;
    line-height: 48px;
    letter-spacing: -1px;
    color: #ffffff;
    padding: 28px;
  }
  &__item {
    border-radius: 8px;
    width: 570px;
    height: 384px;
    position: relative;
    object-fit: cover;
    overflow: hidden;
    cursor: pointer;
    margin-top: 50px;
  }
  &__img {
    width: 100%;
    &:hover {
      transform: scale(1.2);
    }
  }
  &__number-img {
    position: absolute;
    left: 0;
    bottom: 0;
  }
  .heading_sm {
    font-family: "Hind Siliguri";
    font-weight: bold;
    font-size: 24px;
    line-height: 32px;
    color: #333333;
    margin-top: 25px;
  }
  .paragraph {
    font-family: "Work Sans";
    font-size: 16px;
    line-height: 32px;
    color: rgba(51, 51, 51, 0.496405);
    margin-top: 4px;
  }
}
// Responsive styles
@media screen and (max-width: 1200px) {
  .part {
    padding: 20px;

    &__item {
      width: 520px;
      height: auto;
    }
  }
}
@media screen and (max-width: 1100px) {
  .part {
    padding: 20px;
    &__item {
      width: 470px;
      height: auto;
    }
  }
}
@media screen and (max-width: 1000px) {
  .part {
    padding: 20px;
    margin-left: 50%;
    transform: translate(-50%);
    &__item {
      max-width: 570px;
      height: auto;
    }
  }
}
@media screen and (max-width: 1000px) {
  .part {
    &__item {
      max-width: 350px;
    }
  }
}
</style>

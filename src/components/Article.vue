<template>
  <div class="article-card">
    <article class="article-card__item">
      <img :src="img" alt="Article Image" />
    </article>
    <h4 class="heading">{{ title }}</h4>
  </div>
</template>

<style lang="scss">
.article-card {
  max-width: 370px;
  border: 1px solid #e6edf5;
  box-sizing: border-box;
  border-radius: 8px;
  padding: 16px 16px 40px 16px;
  cursor: pointer;
  transition: all 0.5s;
  &:hover {
    box-shadow: 0px 24px 48px rgba(0, 17, 86, 0.0799083);
  }
  &__item {
    border-radius: 8px 8px 50px 8px;
    overflow: hidden;
    object-fit: cover;
    max-width: 370px;
    height: 240px;
    img {
      width: 100%;
      transition: all 0.3s;
      &:hover {
        transform: scale(1.2);
      }
    }
  }
  .heading {
    font-family: "Hind Siliguri";
    font-style: normal;
    font-weight: bold;
    font-size: 24px;
    line-height: 32px;
    color: #333333;
    margin-top: 25px;
  }
}
@media screen and (max-width: 1200px) {
  .article-card {
    width: 340px;
  }
}
@media screen and (max-width: 1100px) {
  .article-card {
    width: 320px;
  }
}
@media screen and (max-width: 1000px) {
  .article-card {
    width: 280px;
    &__item {
      height: 180px;
    }
  }
}
</style>

<script>
export default {
  name: "Article",
  props: ["title", "img"],
};
</script>

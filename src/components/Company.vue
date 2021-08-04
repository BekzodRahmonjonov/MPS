<template>
  <div class="container">
    <div class="company">
      <div class="company__creative-marketing">
        <h5 class="pink-heading">Company</h5>
        <h1 class="company__heading">
          Creative
          <span class="company__heading_underline">Marketing</span>
          <img
            class="company__green-underline"
            src="../assets/green-underline.png"
          />
          <p class="paragraph">
            The sky was cloudless and of a deep dark blue the spectacle before
            us was indeed sublime.
          </p>
          <button class="btn">Explore</button>
        </h1>
      </div>
      <div class="company__img">
        <img class="company__img-item" src="../assets/company-img.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Company",
};
</script>

<style lang="scss">
.company {
  padding: 50px 0;
  display: flex;
  align-items: center;
  justify-content: space-between;
  &__creative-marketing {
    max-width: 470px;
    position: relative;
  }
  &__heading {
    font-family: "Hind Siliguri";
    font-weight: bold;
    font-size: 72px;
    line-height: 80px;
    letter-spacing: -1px;
    color: #333333;
    margin-top: 24px;
    &_underline {
      color: #4db282;
      display: block;
    }
  }
  &__green-underline {
    width: 350px;
    position: absolute;
    top: 200px;
    left: -10px;
  }
  .paragraph {
    margin-top: 55px;
  }
  &__img {
    max-width: 554px;
    &-item {
      width: 100%;
    }
  }
  .btn {
    margin-top: 35px;
  }
}

// Responsive Company
@media screen and (max-width: 1200px) {
  .container {
    max-width: 1140px;
  }
}
</style>

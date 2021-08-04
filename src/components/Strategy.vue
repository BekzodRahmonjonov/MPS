<template>
  <div class="strategy">
    <div class="container">
      <div class="strategy__img">
        <img class="strategy__img-item" src="../assets/stragy-img.png" alt="" />
      </div>
      <div class="strategy__item">
        <h2 class="heading">Strategy, technology and design</h2>
        <p class="paragraph">
          Apparently we had reached a great height in the atmosphere, for the
          sky was a dead black.
        </p>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.strategy {
  background: #f07566;
  padding: 80px 20px;
  margin-top: 100px;
  margin-bottom: 120px;
  .container {
    display: flex;
    justify-content: space-between;
  }
  &__item {
    max-width: 510px;
  }
  &__img {
    width: 180px;
    position: relative;
    &-item {
      position: absolute;
      top: -160px;
      left: 0;
    }
  }
  .heading {
    font-family: "Hind Siliguri";
    font-style: normal;
    font-weight: bold;
    font-size: 56px;
    line-height: 64px;
    letter-spacing: -1px;
    color: #ffffff;
  }
  .paragraph {
    font-family: "Work Sans";
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 32px;
    color: #ffffff;
  }
}
@media screen and (max-width: 900px) {
  .strategy {
    &__item {
      max-width: 370px;
    }
    &__img-item {
      top: -100px;
    }
  }
}
@media screen and (max-width: 768px) {
  .strategy {
    .container {
      flex-direction: column;
      gap: 400px;
      margin-left: 50%;
      transform: translate(-50%);
    }
    &__img-item {
      top: -150px;
    }
  }
}
@media screen and (max-width: 576px) {
  .strategy {
    .container {
      flex-direction: column;
      gap: 400px;
      max-width: 500px;
    }
    &__img-item {
      top: -150px;
    }
  }
}
@media screen and (max-width: 375px) {
  .strategy {
    width: 350px;
    margin: auto;
    &__img-item {
      top: -150px;
      width: 300px;
      left: -60px;
    }
  }
}
</style>

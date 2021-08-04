<template>
  <div class="container">
    <div class="company testimonials">
      <div class="company__img">
        <img
          class="company__img-item"
          src="../assets/testimonials-img.png"
          alt=""
        />
      </div>
      <div class="company__creative-marketing">
        <h5 class="pink-heading">Testimonials</h5>
        <h1 class="company__heading">Reviews</h1>
        <div class="testimonials__card">
          <p class="paragraph">
            "The sky was cloudless and of a deep dark blue the spectacle before
            us was indeed sublime sky was cloudless and of a deep dark."
          </p>
          <h5 class="heading">Jaroslav Brabec</h5>
          <h6 class="heading_sm">Microsoft</h6>
        </div>
        <div class="testimonials__icon">
          <img src="../assets/left.png" alt="" />
          <img src="../assets/rigth.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.testimonials {
  &__card {
    background: #ffffff;
    box-shadow: 0px 24px 48px rgba(0, 17, 86, 0.0799083);
    border-radius: 8px;
    padding: 25px 32px;
  }
  .paragraph {
    font-family: "Work Sans";
    font-size: 16px;
    line-height: 32px;
    color: rgba(51, 51, 51, 0.496405);
  }
  .heading {
    font-family: "Hind Siliguri";
    font-weight: bold;
    font-size: 24px;
    line-height: 32px;
    color: #333333;
    margin-top: 14px;
  }
  .heading_sm {
    font-family: "Work Sans";
    font-size: 14px;
    line-height: 24px;
    color: rgba(51, 51, 51, 0.496405);
    margin-top: 6px;
  }
  &__icon {
    margin-top: 48px;
    display: flex;
    gap: 10px;
    cursor: pointer;
  }
}
@media screen and (max-width: 1100px) {
  .company__img {
    width: 500px;
  }
}
</style>

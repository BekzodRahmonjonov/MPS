<template>
  <div class="container">
    <div class="company service">
      <div class="company__creative-marketing">
        <h5 class="pink-heading">Service</h5>
        <h1 class="company__heading">Marketing and Creative Consulting</h1>
        <p class="paragraph">
          TDistant orb has power to raise and purify our thoughts like a strain
          of sacred music, or a noble picture.
        </p>
        <div class="service__item">
          <div class="clients">
            <div class="clients__item">
              <img src="../assets/icon-1.png" alt="" />
              <div>
                <h2 class="heading">42+</h2>
                <span class="clients__item-span">Clients</span>
              </div>
            </div>
          </div>
          <div class="clients">
            <div class="clients__item">
              <img src="../assets/icon-2.png" alt="" />
              <div>
                <h2 class="heading">75%</h2>
                <span class="clients__item-span">Succeful</span>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="company__img">
        <img class="company__img-item" src="../assets/service-img.png" alt="" />
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.service {
  &__item {
    display: flex;
    align-items: center;
    gap: 90px;
    margin-top: 40px;
    .clients {
      &__item {
        display: flex;
        align-items: center;
        gap: 10px;
        .heading {
          font-family: "Hind Siliguri";
          font-style: normal;
          font-weight: bold;
          font-size: 40px;
          line-height: 48px;
          letter-spacing: -1px;
          color: #333333;
        }
        &-span {
          font-family: "Work Sans";
          font-size: 16px;
          line-height: 32px;
          color: rgba(51, 51, 51, 0.496405);
        }
      }
    }
  }
}
// Responsive styles
@media screen and (max-width: 1000px) {
  .company__creative-marketing,
  .company__img {
    max-width: 440px;
  }
}
@media screen and (max-width: 900px) {
  .company__creative-marketing,
  .company__img {
    max-width: 400px;
  }
}
@media screen and (max-width: 768px) {
  .company {
    flex-direction: column;
    gap: 50px;
  }
  .company__creative-marketing,
  .company__img {
    max-width: 500px;
  }
}
@media screen and (max-width: 375px) {
  .company__creative-marketing,
  .company__img {
    max-width: 350px;
  }
}
</style>

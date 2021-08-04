<template>
  <div class="contact-us">
    <div class="container">
      <div class="contact-us__kickstar">
        <h3 class="heading">Kickstart Your Next Project</h3>
        <button class="btn">Contact Us</button>
      </div>
      <div class="contact-us__paragraph">
        <p class="paragraph">
          I shall see the face of Mars, anyhow, and that will be a rare
          experience. It seems to me that a view of the heavenly bodies through
          a fine telescope, as well as a tour round the world, should form a
          part of a liberal education.
        </p>
      </div>
      <img class="contact-us__img" src="../assets/contactUs-img.png" alt="" />
    </div>
  </div>
</template>

<style lang="scss">
.contact-us {
  padding: 50px 0;
  .container {
    display: flex;
    justify-content: space-between;
    background: #f07566;
    border-radius: 8px;
    padding: 80px 100px 90px;
    position: relative;
  }
  .btn {
    background: #fbd34b;
    color: #333333;
    margin-top: 34px;
  }
  &__kickstar {
    width: 300px;
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
  &__paragraph {
    max-width: 470px;
    .paragraph {
      font-family: "Work Sans";
      font-style: normal;
      font-weight: normal;
      font-size: 16px;
      line-height: 32px;
      color: #ffffff;
      margin-top: 10px;
    }
  }
  &__img {
    position: absolute;
    bottom: -40px;
    left: 50%;
    transform: translate(-50%);
  }
}
@media screen and (max-width: 900px) {
  .contact-us {
    .container {
      padding: 80px 50px;
    }
  }
}
@media screen and (max-width: 768px) {
  .contact-us {
    .container {
      padding-bottom: 130px;
      flex-direction: column;
      gap: 50px;
    }
  }
}
@media screen and (max-width: 375px) {
  .contact-us {
    width: 350px;
  }
}
</style>

<template>
  <div class="container">
    <div class="company-newsletter">
      <h2 class="heading">Company Newsletter</h2>
      <div class="company-newsletter__forms">
        <input
          type="email"
          class="company-newsletter__input"
          placeholder="Your Email"
        />
        <button class="btn">Subscribe</button>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.company-newsletter {
  padding: 50px 0;
  margin: 50px 0;
  display: flex;
  align-items: center;
  justify-content: space-between;
  .heading {
    font-family: "Hind Siliguri";
    font-weight: bold;
    font-size: 40px;
    line-height: 48px;
    letter-spacing: -1px;
    color: #333333;
  }
  &__forms {
    display: flex;
    gap: 30px;
  }
  &__input {
    border: 1px solid #dadada;
    border-radius: 6px;
    outline: #dadada;
    padding: 16px;
    &::placeholder {
      font-family: "Work Sans";
      font-size: 16px;
      line-height: 32px;
      color: rgba(51, 51, 51, 0.496405);
    }
  }
}
@media screen and (max-width: 576px) {
  .company-newsletter {
    flex-direction: column;
    gap: 50px;
    &__forms {
      flex-direction: column;
      gap: 30px;
    }
  }
}
</style>

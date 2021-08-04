<template>
  <div class="container">
    <div class="partners">
      <img src="../assets/partners-1.png" alt="" />
      <img src="../assets/partners-2.png" alt="" />
      <img src="../assets/partners-3.png" alt="" />
      <img src="../assets/partners-4.png" alt="" />
      <img src="../assets/partners-5.png" alt="" />
      <img src="../assets/partners-6.png" alt="" />
    </div>
  </div>
</template>

<style lang="scss">
.partners {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
  padding: 80px 20px;
}
@media screen and (max-width: 576px) {
  .partners {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 30px;
  }
}
</style>

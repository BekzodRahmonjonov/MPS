<template>
  <div class="container">
    <header class="header">
      <router-link to="/home">
        <img src="../assets/logo.png" alt="Logo" />
      </router-link>
      <ul class="header__menu" :class="burgerOpen ? 'menu-show' : ''">
        <li class="list">
          <a class="link">About</a>
        </li>
        <li class="list">
          <a class="link">Portfolio</a>
        </li>
        <li class="list">
          <a class="link">Service</a>
        </li>
        <li class="list">
          <a class="link">Blog</a>
        </li>
        <li class="list">
          <a class="link">Contact</a>
        </li>
      </ul>
      <button class="btn-white">Contact</button>
      <button class="openBurger-btn" @click="burger()">
        <img src="../assets/menu-open.png" class="burger-open" />
      </button>
    </header>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      burgerOpen: false,
    };
  },
  methods: {
    burger() {
      this.burgerOpen = !this.burgerOpen;
    },
  },
};
</script>

<style lang="scss">
.header {
  display: grid;
  align-items: center;
  padding: 16px 0;
  // position: fixed;
  // top: 0;
  // left: 0;
  // right: 0;
  grid-template-columns: 1fr 2fr 3fr;
  &__menu {
    display: flex;
    align-items: center;
    gap: 40px;
    .link {
      font-family: "Work Sans";
      line-height: 32px;
      color: #333333;
    }
  }
  .burger-open {
    display: none;
  }
  .openBurger-btn {
    background-color: transparent;
    border: none;
    outline: none;
  }
}

// Responsive styles
@media screen and (max-width: 1200px) {
  .header {
    padding: 16px 30px;
  }
}
@media screen and (max-width: 768px) {
  .header {
    padding: 16px 30px;
    display: flex;
    justify-content: space-between;
    // position: relative;
    &__menu {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      flex-direction: column;
      top: 100px;
      left: -100%;
      transition: 0.5s;
      width: 100%;
      height: 600px;
      padding: 50px;
      z-index: 100;
      background-color: rgb(219, 218, 218);
      .link {
        font-size: 30px;
      }
    }
    .menu-show {
      left: 0;
    }

    .btn-white {
      display: none;
      position: absolute;
      top: 500px;
      left: 50%;
      transform: translate(-50%);
      z-index: 20;
    }
    .burger-open {
      display: block;
    }
  }
}
</style>

<template>
  <div class="container">
    <div class="company about">
      <div class="company__img">
        <img class="company__img-item" src="../assets/about-img.png" alt="" />
      </div>
      <div class="company__creative-marketing about__item">
        <h5 class="pink-heading">About</h5>
        <h1 class="heading">We Build PRO Business</h1>
        <h4 class="heading_sm">Excited to work with customers</h4>
        <p class="paragraph paragraph_first">
          <svg
            width="24"
            height="22"
            viewBox="0 0 24 22"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M22 11C22 10.421 21.942 9.857 21.856 9.303L19.99 11.205C19.879 16.072 15.894 20 11 20C6.038 20 2 15.962 2 11C2 6.038 6.038 2 11 2C12.8 2 14.474 2.537 15.882 3.45L17.304 1.993C15.518 0.741 13.347 0 11 0C4.925 0 0 4.925 0 11C0 17.075 4.925 22 11 22C17.075 22 22 17.075 22 11ZM11.5 10.806L20.904 1.167L24 4.263L11.5 17L4.562 10.29L7.657 7.192L11.5 10.806Z"
              fill="#4DB282"
            />
          </svg>
          <span>The sky was cloudless and of a deep</span>
        </p>
        <p class="paragraph">
          <svg
            width="24"
            height="22"
            viewBox="0 0 24 22"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M22 11C22 10.421 21.942 9.857 21.856 9.303L19.99 11.205C19.879 16.072 15.894 20 11 20C6.038 20 2 15.962 2 11C2 6.038 6.038 2 11 2C12.8 2 14.474 2.537 15.882 3.45L17.304 1.993C15.518 0.741 13.347 0 11 0C4.925 0 0 4.925 0 11C0 17.075 4.925 22 11 22C17.075 22 22 17.075 22 11ZM11.5 10.806L20.904 1.167L24 4.263L11.5 17L4.562 10.29L7.657 7.192L11.5 10.806Z"
              fill="#4DB282"
            />
          </svg>
          <span>Spectacle before us was indeed </span>
        </p>
        <p class="paragraph">
          <svg
            width="24"
            height="22"
            viewBox="0 0 24 22"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M22 11C22 10.421 21.942 9.857 21.856 9.303L19.99 11.205C19.879 16.072 15.894 20 11 20C6.038 20 2 15.962 2 11C2 6.038 6.038 2 11 2C12.8 2 14.474 2.537 15.882 3.45L17.304 1.993C15.518 0.741 13.347 0 11 0C4.925 0 0 4.925 0 11C0 17.075 4.925 22 11 22C17.075 22 22 17.075 22 11ZM11.5 10.806L20.904 1.167L24 4.263L11.5 17L4.562 10.29L7.657 7.192L11.5 10.806Z"
              fill="#4DB282"
            />
          </svg>
          <span>Cloudless and of a deep dark</span>
        </p>
        <div class="btn">Learn more</div>
      </div>
    </div>
    <div class="aboutCard-component">
      <aboutCard
        v-for="(item, index) in aboutCardArticle"
        :key="index"
        :heading="item.heading"
        :img="item.img"
        :paragraph="item.paragraph"
      />
    </div>
  </div>
</template>

<script>
import aboutCard from "./aboutCard.vue";
export default {
  components: {
    aboutCard,
  },
  data() {
    return {
      aboutCardArticle: [
        {
          img: "https://picsum.photos/64/64",
          heading: "Consulting",
          paragraph:
            "The sky was cloudless and of a deep dark blue the spectacle before.",
        },
        {
          img: "https://picsum.photos/64/64",
          heading: "Planning",
          paragraph:
            "Apparently we had reached a great height in the atmosphere.",
        },
        {
          img: "https://picsum.photos/64/64",
          heading: "Support",
          paragraph:
            "By the same illusion which lifts the horizon of the sea to the level.",
        },
        {
          img: "https://picsum.photos/64/64",
          heading: "Cooperation",
          paragraph:
            "Spectator on a hillside, the sable cloud beneath was dished out.",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.about {
  &__item {
    max-width: 350px;
  }
  .heading {
    font-family: "Hind Siliguri";
    font-style: normal;
    font-weight: bold;
    font-size: 56px;
    line-height: 64px;
    letter-spacing: -1px;
    color: #333333;
    margin-top: 20px;
  }
  .heading_sm {
    font-family: "Hind Siliguri";
    font-style: normal;
    font-weight: bold;
    font-size: 24px;
    line-height: 32px;
    color: #333333;
    opacity: 0.9;
    margin-top: 26px;
  }
  .paragraph {
    font-family: "Work Sans";
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    line-height: 32px;
    color: #333333;
    display: flex;
    align-items: center;
    gap: 10px;
    margin-top: 10px;
    &_first {
      margin-top: 40px;
    }
  }
  .btn {
    width: 188px;
    margin-top: 42px;
  }
}
.aboutCard-component {
  display: flex;
  justify-content: space-between;
  margin: 120px 0;
}
@media screen and (max-width: 1100px) {
  .aboutCard-component {
    gap: 20px;
  }
}
@media (min-width: 769) and (max-width: 900px) {
  .aboutCard-component {
    display: grid;
    grid-template-columns: 1fr 1fr;
  }
  .about-card {
    max-width: 320px;
    margin-left: 50%;
    transform: translate(-50%);
    margin-top: 50px;
  }
}
@media screen and (max-width: 768px) {
  .aboutCard-component {
    display: felx;
    flex-direction: column;
  }
  .about-card {
    width: 400px;
    margin: 0 auto;
    transform: translate(0);
    margin-top: 50px;
  }
}
@media screen and (max-width: 375px) {
  .about-card {
    width: 350px;
  }
}
</style>

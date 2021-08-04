<template>
  <div class="container">
    <div class="portfolio">
      <h6 class="pink-heading">Portfolio</h6>
      <h2 class="heading">Company Cases</h2>
      <p class="paragraph">
        Apparently we had reached a great height in the atmosphere, for the sky
        was a dead black, and the stars had ceased to twinkle the same illusion
        which lifts the horizon of the sea.
      </p>
      <div class="portfolio__card">
        <PortfolioCard
          v-for="(item, index) in PortfolioCardData"
          :key="index"
          :img="item.img"
          :heading="item.heading"
          :paragraph="item.paragraph"
          :number="item.number"
        />
      </div>
      <button class="btn-white">Browse all</button>
    </div>
  </div>
</template>

<script>
import PortfolioCard from "../components/PortfolioCard.vue";

export default {
  components: {
    PortfolioCard,
  },
  data() {
    return {
      PortfolioCardData: [
        {
          img: "https://picsum.photos/570/384",
          number: "01",
          heading: "Face of Mars",
          paragraph: "Will be a rare experience",
        },
        {
          img: "https://picsum.photos/570/384",
          number: "02",
          heading: "Heavenly Bodies",
          paragraph: "Tour round the world should form",
        },
        {
          img: "https://picsum.photos/570/384",
          number: "03",
          heading: "Liberal Education",
          paragraph: "Truly it was a great journey",
        },
        {
          img: "https://picsum.photos/570/384",
          number: "04",
          heading: "Though the Gravity",
          paragraph: "Daily classes he no longer collapsed",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.portfolio {
  margin: 120px 0;
  .pink-heading {
    display: inline-block;
    margin-left: 50%;
    transform: translate(-50%);
  }
  .heading {
    font-family: "Hind Siliguri";
    font-weight: bold;
    font-size: 56px;
    line-height: 64px;
    text-align: center;
    letter-spacing: -1px;
    color: #333333;
    margin-top: 20px;
  }
  .paragraph {
    max-width: 770px;
    font-family: "Work Sans";
    font-size: 16px;
    line-height: 32px;
    text-align: center;
    color: rgba(51, 51, 51, 0.496405);
    margin: 0 auto;
    margin-top: 28px;
  }
  .btn-white {
    margin-left: 50%;
    transform: translate(-50%);
    margin-top: 80px;
  }
}
.portfolio__card {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  margin: 30px 0;
}
.articles {
  gap: 15px;
}
@media screen and (max-width: 768px) {
  .portfolio {
    margin: 0;
  }
}
</style>

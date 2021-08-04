<template>
  <div class="container">
    <div class="latest">
      <div class="latest__header">
        <h5 class="pink-heading">Latest articles</h5>
        <h2 class="heading">Check Our Insights</h2>
        <p class="paragraph">
          See the face of Mars, anyhow, and that will be a rare experience seems
          to me that a view of the heavenly bodies through a fine telescope, as
          well as a tour round the world.
        </p>
      </div>
      <div class="latest__card">
        <div class="latest__card-img">
          <img src="https://picsum.photos/560/340" />
        </div>
        <div class="latest__card-item">
          <div class="heading">
            What looked like a small patch of purple grass
          </div>
          <p class="paragraph">
            Truly it was a great journey, and in it I met with many, whom to
            know was to love.
          </p>
        </div>
      </div>
      <div class="articles">
        <Article
          v-for="(item, index) in article"
          :key="index"
          :img="item.img"
          :title="item.title"
        />
      </div>
      <button class="btn-white">Browse all</button>
    </div>
  </div>
</template>

<script>
import Article from "./Article.vue";
export default {
  data() {
    return {
      article: [
        {
          img: "https://picsum.photos/340/240",
          title: "Above five feet square, was moving across",
        },
        {
          img: "https://picsum.photos/340/240",
          title: "Enough he perceived that it was not grass",
        },
        {
          img: "https://picsum.photos/340/240",
          title: "There were no blades, but only purple roots",
        },
      ],
    };
  },
  components: {
    Article,
  },
};
</script>

<style lang="scss">
.latest {
  padding: 50px 0;
  &__header {
    text-align: center;
    max-width: 770px;
    margin: 0 auto;
    .pink-heading {
      display: inline-block;
      &::before {
        right: 0;
      }
    }
    .heading {
      font-family: "Hind Siliguri";
      font-weight: bold;
      font-size: 56px;
      line-height: 64px;
      letter-spacing: -1px;
      margin-top: 20px;
    }
    .paragraph {
      font-family: "Work Sans";
      font-size: 16px;
      line-height: 32px;
      color: rgba(51, 51, 51, 0.496405);
      margin-top: 28px;
    }
  }
  &__card {
    margin-top: 45px;
    border: 1px solid #e6edf5;
    border-radius: 8px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 16px 40px 16px 16px;
    &-item {
      max-width: 480px;
      .heading {
        font-family: "Hind Siliguri";
        font-weight: bold;
        font-size: 40px;
        line-height: 48px;
        letter-spacing: -1px;
        color: #333333;
      }
      .paragraph {
        font-family: "Work Sans";
        font-size: 20px;
        line-height: 32px;
        color: #333333;
        margin-top: 30px;
      }
    }
    &-img {
      max-width: 554px;
      height: 336px;
      border-radius: 8px 8px 50px 8px;
      overflow: hidden;
      img {
        width: 100%;
        object-fit: cover;
        transition: all 0.3s;
        &:hover {
          transform: scale(1.2);
        }
      }
    }
  }
  .btn-white {
    margin-top: 64px;
    margin-left: 50%;
    transform: translate(-50%);
  }
}
.articles {
  display: flex;
  justify-content: space-between;
  margin-top: 32px;
}
@media screen and (max-width: 1100px) {
  .latest {
    &__card-img {
      max-width: 470px;
    }
    &__card-item {
      max-width: 420px;
    }
  }
}
@media screen and (max-width: 1000px) {
  .latest {
    &__card-img {
      max-width: 440px;
    }
    &__card-item {
      max-width: 350px;
    }
  }
}
@media screen and (max-width: 900px) {
  .latest {
    &__card-img {
      max-width: 400px;
      height: auto;
    }
    &__card-item {
      max-width: 350px;
    }
  }
}
@media screen and (max-width: 768px) {
  .latest {
    &__card {
      flex-direction: column;
      gap: 50px;
      padding-top: 20px;
      padding-bottom: 20px;
    }
  }
  .articles {
    flex-direction: column;
    .article-card {
      max-width: 420px;
      margin: 0 auto;
      margin-top: 50px;
    }
  }
}
</style>

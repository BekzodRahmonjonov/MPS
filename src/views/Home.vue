<template>
  <div class="home">
    <Header />
    <Company />
    <About />
    <Features />
    <Portfolio />
    <Partners />
    <Service />
    <Strategy />
    <Testimonials />
    <ContactUs />
    <CompanyNewsletter />
    <LatestArticles />
    <Footer />
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import Company from "../components/Company.vue";
import Testimonials from "../components/Testimonials.vue";
import About from "../components/About.vue";
import Features from "../components/Features.vue";
import Partners from "../components/Partners.vue";
import Service from "../components/Service.vue";
import Strategy from "../components/Strategy.vue";
import ContactUs from "../components/ContactUs.vue";
import CompanyNewsletter from "../components/CompanyNewsletter.vue";
import LatestArticles from "../components/LatestArticles.vue";
import Footer from "../components/Footer.vue";
import Portfolio from "../components/Portfolio.vue";

export default {
  components: {
    Header,
    Company,
    Testimonials,
    About,
    Features,
    Partners,
    Service,
    Strategy,
    ContactUs,
    CompanyNewsletter,
    LatestArticles,
    Footer,
    Portfolio,
  },
};
</script>

<style lang="scss">
// Import Fotns
@import url("https://fonts.googleapis.com/css2?family=Hind+Siliguri:wght@300;400;500;600;700&family=Work+Sans:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

// Styles
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.container {
  max-width: 1200px;
  margin: 0 auto;
}
.link {
  text-decoration: none;
  color: #000;
  cursor: pointer;
}
.list {
  list-style: none;
}
.btn {
  font-family: "Hind Siliguri";
  font-weight: bold;
  font-size: 16px;
  line-height: 26px;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: #ffffff;
  background: #f07566;
  border-radius: 6px;
  outline: none;
  border: none;
  cursor: pointer;
  padding: 11px 40px;
  &:hover {
    opacity: 0.5;
  }
}
.btn-white {
  font-family: "Hind Siliguri";
  font-weight: bold;
  font-size: 16px;
  line-height: 26px;
  letter-spacing: 1px;
  color: #f07566;
  text-transform: uppercase;
  background-color: #ffffff;
  border: 1px solid rgba(240, 117, 102, 0.236809);
  border-radius: 6px;
  outline: none;
  padding: 11px 32px;
  margin: 0 auto;
  margin-right: 100px;
  cursor: pointer;
  &:hover {
    opacity: 0.5;
  }
}
.pink-heading {
  font-family: "Hind Siliguri";
  font-weight: bold;
  font-size: 16px;
  line-height: 32px;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: #f07566;
  position: relative;
  margin-left: 20px;
  &::before {
    content: "";
    display: block;
    height: 12px;
    width: 12px;
    border-radius: 50%;
    background: #f07566;
    position: absolute;
    left: -20px;
    top: 9px;
  }
}
.scroll-none {
  overflow: scroll;
}
.paragraph {
  font-family: "Work Sans";
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 32px;
  color: #333333;
}
// Responsive Styles
@media screen and (max-width: 1200px) {
  .container,
  .footer-foot {
    max-width: 1140px;
  }
}
@media screen and (max-width: 1100px) {
  .container,
  .footer-foot {
    max-width: 1040px;
  }
}
@media screen and (max-width: 1000px) {
  .container,
  .footer-foot {
    max-width: 940px;
  }
}
@media screen and (max-width: 900px) {
  .container,
  .footer-foot {
    max-width: 840px;
    padding: 20px 0;
  }
}
@media screen and (max-width: 800px) {
  .container,
  .footer-foot {
    max-width: 740px;
  }
}
@media screen and (max-width: 768px) {
  .container {
    max-width: 720px;
  }
}
@media screen and (max-width: 576px) {
  .container {
    max-width: 540px;
  }
}
@media screen and (max-width: 375px) {
  .container {
    max-width: 350px;
    margin: auto;
  }
}
</style>

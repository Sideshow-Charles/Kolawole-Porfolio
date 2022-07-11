<template>
  <div id="landing__page">
    <Header></Header>
    <article class="article__container">
      <article class="article__header">
        <p>
          Product designer who is passionate about solving problems and creating
          the best user experiences.
        </p>
      </article>
      <article class="article__text">
        <p>
          Hi, I’m Kolawole Popoola, a Product Designer with over 4 years
          experience in delivering end to end, usable designs for digital
          products. I currently work with some talented people at
          <span><a href="http://kuda.com/">Kuda Bank</a></span>
          building the best Neobank in Africa. In my spare time, I write about
          sports, I watch a lot of sports and I play video games.
        </p>
      </article>
      <article class="article-CTA__link">
        <p>
          <a href="/about">Read more about me</a>
          <img src="../assets/images/underline.svg" alt="" />
        </p>
      </article>
    </article>

    <div class="button__container">
      <Button btn-style="mobile"></Button>
    </div>

    <section class="section__container">
      <section class="section__content">
        <section class="section__header">
          <p>Some of my selected work</p>
        </section>
        <section class="selected-works__container">
          <!-- <div class="selected__works"> -->
          <a href="/kuda-business-banking"
            ><img src="../assets/images/selected-work1.png" alt=""
          /></a>
          <a href="/monthly"
            ><img src="../assets/images/selected-work2.png" alt=""
          /></a>
          <!-- </div> -->

          <!-- <div class="selected__works"> -->
          <a href="/citrone"
            ><img src="../assets/images/selected-work3.png" alt=""
          /></a>
          <a href="/coded-agents"
            ><img src="../assets/images/selected-work4.png" alt=""
          /></a>
          <!-- </div> -->
        </section>

        <!-- Mobile Images -->

        <section class="selected-works__container__mobile">
          <div class="selected__works__mobile">
            <a href="/kuda-business-banking"
              ><img src="../assets/images/mobile-image-kuda.png" alt=""
            /></a>
            <a href="/monthly"
              ><img src="../assets/images/mobile-image-monthly.png" alt=""
            /></a>
          </div>

          <div class="selected__works__mobile">
            <a href="/citrone"
              ><img src="../assets/images/mobile-image-citrone.png" alt=""
            /></a>
            <a href="/coded-agents"
              ><img src="../assets/images/mobile-image-coded-agents.png" alt=""
            /></a>
          </div>
        </section>

        <!-- End Of Mobile Images -->
      </section>
    </section>
    <div id="landing__page">
      <section class="sub-footer__container">
        <section class="sub-footer__text">
          <p>
            Want to build something ground breaking and you feel I might <br />
            be the right fit? What are you waiting for
          </p>
        </section>
        <Button></Button>
      </section>

      <Footer></Footer>
    </div>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import Button from "../components/Button.vue";
import Footer from "../components/Footer.vue";
export default {
  components: {
    Header,
    Button,
    Footer,
  },
};
</script>

<style scoped>
#landing__page {
  background-image: url("../assets/images/lines-for-web.svg");
  background-repeat: repeat-y;
  background-position: top center;
}

.article__container {
  max-width: 109.2rem;
  margin: 0 auto;
  padding-top: 7rem;
  padding-bottom: 5rem;
  padding-left: 121px;
  padding-right: 121px;
}

.article__header {
  font-family: "Graphik-SemiBold";
  font-size: 2rem;
  font-weight: 300;
  line-height: 4.5rem;
  margin-bottom: 2rem;
  max-width: 57rem;
}

.article__text {
  font-family: "Graphik-Regular";
  font-size: 1.3rem;
  font-weight: 300;
  line-height: 3.2rem;
  margin-bottom: 2.5rem;
  max-width: 54rem;
}

.article__text p span {
  text-decoration: underline;
  font-weight: 900;
  font-family: "Graphik-Medium";
}

.article-CTA__link {
  font-family: "Graphik-Medium";
  font-size: 1.3rem;
  font-weight: 300;
  width: fit-content;
  position: relative;
}

.article-CTA__link img {
  position: absolute;
  left: 0;
  bottom: -10px;
}

.article-CTA__link a {
  text-decoration: none;
  color: inherit;
}

.button__container {
  display: none;
}

.section__container {
  background: #f0f8fb;
  padding: 64px 0;
}

.section__content {
  max-width: 109.2rem;
  margin: 0 auto;
  padding-left: 121px;
  padding-right: 121px;
}

.section__header {
  font-size: 1.5rem;
  font-weight: 900;
  font-family: "Graphik-Medium";
  margin-bottom: 3rem;
  line-height: 2.4rem;
}

.selected-works__container {
  gap: 72px;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(370px, 1fr));
  /* overflow: hidden; */
}

.selected-works__container__mobile {
  display: none;
}

.selected-works__container a img {
  max-width: 100%;
  transition: transform 0.5s ease;
  /* overflow: hidden; */
}

.selected-works__container a img:hover {
  transform: scale(1.02);
  /* overflow: hidden; */
}

.selected-works__container a {
  /* width: fit-content; */
  /* display: inline-block; */
}

/* .selected__works {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
} */

.sub-footer__container {
  text-align: center;
  padding: 10rem 144px;
}

.sub-footer__text {
  margin-bottom: 2rem;
  line-height: 1.8;
  font-size: 1.5rem;
  font-weight: 500;
  font-family: "Graphik-Medium";
}

@media screen and (min-width: 1600px) {
  /* #landing__page {
    background-image: url("../assets/images/lines-for-web.svg");
    background-repeat: repeat-x;
    background-position: top center;
  } */

  .selected-works__container {
    gap: 72px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(550px, 1fr));
  }
}

@media screen and (max-width: 1280px) {
  .selected-works__container {
    gap: 72px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
  }

  /* .selected-works__container a img {
    max-width: 500px;
  } */
}

@media screen and (max-width: 1024px) {
  .selected-works__container {
    gap: 60px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  }
}

@media screen and (max-width: 980px) {
  .article__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .section__content {
    padding-left: 64px;
    padding-right: 64px;
  }

  .selected__works {
    flex-direction: column;
  }

  /* .selected-works__container a img {
    max-width: 100%;
    margin-bottom: 72px;
  } */
}

@media screen and (max-width: 820px) {
  /* .selected-works__container a img {
    max-width: 100%;
  } */
}

@media screen and (max-width: 768px) {
  .article__container {
    padding-left: 32px;
    padding-right: 32px;
  }

  .article-CTA__link img {
    bottom: 0;
    max-width: 190px;
  }

  .section__content {
    padding-left: 32px;
    padding-right: 32px;
  }

  .sub-footer__container {
    padding: 7rem 64px;
  }

  @media screen and (max-width: 540px) {
    #landing__page {
      background-image: url("../assets/images/lines-for-mobile.svg");
      background-repeat: no-repeat;
      background-position: top center;
      height: 100%;
    }

    .article__container {
      padding-top: 41px;
      padding-bottom: 0;
    }

    .article__header {
      font-size: 26px;
      font-weight: 300;
      line-height: 50px;
    }

    .article__text {
      font-size: 18px;
      font-weight: 300;
      line-height: 43px;
    }

    .article-CTA__link {
      font-size: 19px;
      line-height: 43px;
    }

    .button__container {
      display: block;
      padding: 0 32px;
      margin: 50px 0;
    }

    .section__header {
      font-size: 18px;
      font-weight: 300;
      line-height: 43px;
    }

    .sub-footer__text {
      line-height: 43px;
      font-size: 20.5px;
      font-weight: 300;
    }

    .selected-works__container {
      display: none;
    }

    .selected-works__container__mobile {
      display: block;
    }

    .selected-works__container__mobile a img {
      max-width: 100%;
      margin-bottom: 72px;
    }
  }
}

@media screen and (max-width: 320px) {
  .article__header {
    font-size: 20px;
    font-weight: 300;
    line-height: 40px;
  }

  .article__text {
    font-size: 15px;
    font-weight: 300;
    line-height: 40px;
  }

  .article-CTA__link {
    font-size: 16px;
    line-height: 43px;
  }

  .article-CTA__link img {
    bottom: 0;
    max-width: 155px;
  }

  .sub-footer__container {
    padding-left: 32px;
    padding-right: 32px;
  }

  .sub-footer__text {
    font-size: 16px;
    font-weight: 300;
    line-height: 43px;
  }
}

@media screen and (max-width: 280px) {
  .article__container {
    padding-left: 16px;
    padding-right: 16px;
  }

  .button__container {
    padding: 0 16px;
  }

  .section__content {
    padding: 0 16px;
  }

  .sub-footer__text {
    font-size: 14px;
    font-weight: 300;
    line-height: 40px;
  }
}
</style>

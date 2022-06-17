<template>
  <div>
    <Header></Header>
    <article class="article__container">
      <article class="article__header">
        <h1>
          Product designer who is passionate about solving problems and creating
          the best user experiences.
        </h1>
      </article>
      <article class="article__text">
        <p>
          Hi, I’m Kolawole Popoola, a Product Designer with over 4 years
          experience in delivering end to end, usable designs for digital
          products. I currently work with some talented people at
          <span>Kuda Bank</span>
          building the best Neobank in Africa. In my spare time, I write about
          sports, I watch a lot of sports and I play video games.
        </p>
      </article>
      <article class="article-CTA__link">
        <p>Read more about me</p>
      </article>
    </article>
    <section class="section__container">
      <section class="section__content">
        <section class="section__header">
          <p>Some of my selected work</p>
        </section>
        <section class="selected-works__container">
          <a href="/kuda-business-banking"><img src="../assets/images/selected-work1.png" alt="" /></a>
          <a href="/monthly"><img src="../assets/images/selected-work2.png" alt="" /></a>
          <a href="/citrone"><img src="../assets/images/selected-work3.png" alt=""/></a>
          <img src="../assets/images/selected-work4.png" alt="" />
        </section>
      </section>
    </section>

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
</template>

<script>
import Header from "../components/Header.vue";
import Footer from "../components/Footer.vue";
export default {
  components: {
    Header,
    Footer,
  },
};
</script>

<style scoped>
.article__container {
  /* display: flex; */
  flex-direction: column;
  /* justify-content: space-between; */
  max-width: 109.2rem;
  margin: 0 auto;
  padding-top: 5rem;
  padding-bottom: 5rem;
  padding-left: 128px;
  padding-right: 128px;
}

.article__header {
  font-family: "Graphik-Bold";
  font-size: 2rem;
  font-weight: 300;
  letter-spacing: -0.03em;
  line-height: 4.5rem;
  /* margin-bottom: 3rem; */
  max-width: 55rem;
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
  font-family: "Graphik-Regular";
  font-size: 1.3rem;
  font-weight: 300;
}

.section__container {
  background: #f0f8fb;
  padding: 64px 0;
}

.section__content {
  max-width: 109.2rem;
  margin: 0 auto;
  padding-left: 128px;
  padding-right: 128px;
}

.section__header {
  font-size: 1.5rem;
  font-weight: 900;
  font-family: "Graphik-Medium";
  margin-bottom: 3rem;
  line-height: 2.4rem;
}

.selected-works__container {
  display: flex;
  flex-wrap: wrap;
}

.selected-works__container img {
  width: 520px;
  margin-bottom: 72px;
  /* width: 100%; */
}

.selected-works__container img:nth-child(1) {
  margin-right: 72px;
}

.selected-works__container img:nth-child(3) {
  margin-right: 72px;
}

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
  .selected-works__container img {
    width: 800px;
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
}

@media screen and (max-width: 820px) {
  .selected-works__container img {
    width: 100%;
  }
}

@media screen and (max-width: 768px) {
  .article__container {
    padding-left: 32px;
    padding-right: 32px;
  }

  .section__content {
    padding-left: 32px;
    padding-right: 32px;
  }

  .selected-works__container {
    flex-direction: column;
  }

  .selected-works__container img {
    width: 100%;
  }

  .selected-works__container img:nth-child(1) {
    margin-right: 0;
  }

  .selected-works__container img:nth-child(3) {
    margin-right: 0;
  } 

  .sub-footer__container {
    padding: 7rem 64px;
  }
}
</style>

<template>
  <div class="landing__page">
    <Header></Header>
    <article class="about__container">
      <article class="image__container">
        <img src="../assets/images/hero-image.png" alt="" class="hero__image" />

        <div class="contact__container">
          <h3>Contact Me</h3>

          <p>kolapopoola4@gmail.com</p>
        </div>

        <div class="social-images__container">
          <img src="../assets/images/twitter.svg" alt="" />
          <img src="../assets/images/linkedin.svg" alt="" />
        </div>
      </article>

      <article class="about-text__container">
        <article class="about-text__header">
          <p class="about__header">Hello Again</p>
        </article>
        <article class="about-text__container">
          <p>
            I’m Kolawole, a product designer passionate about building
            human-centric products. I currently work at
            <span>Kuda Bank</span> as a Product Designer with some really
            talented people, building one of the biggest Neo-bank’s in Africa.
            Previously I worked at <span>MAX.NG</span> as the Lead Designer.
          </p>
          <p>
            Before joining MAX I worked at
            <span>Fieldinsight.co</span> (Delivery Science) - A logistics
            company built to strengthen companies bonds with their customers
            with a platform that works online and offline that helps your team
            on the field.
          </p>
          <p>
            My journey in design has been a very interesting one, I’ve been
            opportuned to work with great minds and in different fields such as
            fintech, transportation, agritech and also the health sector,
            working in these numerous fields and enivironments has helped me
            ship out great and most importantly usable products. I finished
            university in 2018 with a degree in Computer Science.
          </p>
          <p>
            In my spare time, I write about sports, I watch a lot of sports and
            I play video games. I’m currently available for any design gigs, if
            you’d like to build something groundbreaking shoot me a mail at
            kolapopoola4@gmail.com :)
          </p>
        </article>
      </article>
    </article>

    <section class="section__container">
      <section class="section__toolkit">
        <h2>My Toolkit</h2>

        <section class="section-design__toolkit">
          <div class="design__methods">
            <h3>UX Design Methods</h3>
            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span
              >Wireframing
            </li>
            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span
              >Sketching
            </li>
            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span>User
              Personas
            </li>
            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span>User
              Flows
            </li>
            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span
              >Prototyping
            </li>
            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span>UX
              Thinking
            </li>
          </div>

          <div class="design__tools">
            <h3>UI Design Tools</h3>

            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span
              >Figma
            </li>
            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span
              >Adobe XD
            </li>
            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span
              >Sketch
            </li>
            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span
              >Principle
            </li>
            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span
              >Whimsical
            </li>
            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span
              >Invision Studio
            </li>
          </div>
        </section>
      </section>

      <section class="section-work__history">
        <h2>Work History</h2>
        <section class="section__history">
          <div class="work__history">
            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span>Kuda
              Bank
            </li>
            <p class="role">Product Designer</p>
            <p class="time">2021 - Present</p>

            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span
              >MAX.NG
            </li>
            <p class="role">Lead Product Designer</p>
            <p class="time">2019 - 2021</p>

            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span
              >Delivery Science
            </li>
            <p class="role">Product Designer</p>
            <p class="time">2018-2019</p>
          </div>

          <div class="parkway-projects-work__history">
            <li>
              <span><img src="../assets/images/Polygon.png" alt="" /></span
              >Parkway Projects
            </li>
            <p class="role">UX Designer</p>
            <p class="time">2018-2018</p>
          </div>
        </section>
      </section>
    </section>

    <section class="section-interest__container">
      <div class="section-interest__reading">
        <h3>Currently Reading</h3>
        <img src="../assets/images/currently-reading1.png" alt="" />
        <img src="../assets/images/currently-reading2.png" alt="" />
        <img src="../assets/images/currently-reading3.png" alt="" />
      </div>
      <div class="section-interest__listening">
        <h3>Currently Listening</h3>
        <h6>Podcasts:</h6>
        <img src="../assets/images/currently-listening1.png" alt="" />
        <img src="../assets/images/currently-listening2.png" alt="" />
        <img src="../assets/images/currently-listening3.png" alt="" />
        <img src="../assets/images/currently-listening4.png" alt="" />

        <div class="section-interest__listening__music">
          <h6>Music:</h6>
          <img src="../assets/images/currently-listening5.png" alt="" />
        </div>
      </div>
    </section>
    <SubFooter></SubFooter>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import SubFooter from "../components/SubFooter.vue";
export default {
  components: {
    Header,
    SubFooter,
  },
};
</script>

<style scoped>
.landing__page {
  background-image: url("../assets/images/lines-for-web.svg");
  background-repeat: repeat-y;
  background-position: top center;
}

.about__container {
  padding: 7rem 121px;
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin: 0 auto;
  max-width: 109.2rem;
}

.about-text__container {
  line-height: 2.5rem;
  width: 35rem;
}

.about-text__container p span {
  text-decoration: underline;
}

.image__container {
  display: flex;
  justify-content: space-between;
  flex-direction: column;
}

.image__container img {
  /* height: 50%; */
  margin-bottom: 5rem;
}

.hero__image {
  width: 75%;
}

.contact__container h3 {
  font-family: "Graphik-Medium";
  font-size: 25px;
  font-weight: 900;
  line-height: 60px;
  letter-spacing: 0em;
  text-align: left;
}

.contact__container p {
  font-family: "Graphik-Regular";
  font-size: 16px;
  font-weight: 400;
  line-height: 40px;
  letter-spacing: 0em;
  text-align: left;
}

.social-images__container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 20%;
  margin-top: 2rem;
}

.about-text__header {
  font-family: "Graphik-SemiBold";
  font-size: 2.5rem;
  font-weight: 600;
  line-height: 4.5rem;
  margin-bottom: 2rem;
}

.about-text__container {
  font-family: "Graphik-Regular";
  font-size: 1.3rem;
  font-weight: 300;
  line-height: 3.2rem;
}

.about-text__container p {
  margin-bottom: 3rem;
}

.about-text__container p span {
  text-decoration: underline;
}

.section__container {
  margin: 0 auto;
  max-width: 109.2rem;
  padding-top: 5rem;
  padding-bottom: 7rem;
  padding-left: 121px;
  padding-right: 121px;
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
}

.section__toolkit h2 {
  font-weight: 900;
  font-family: "Graphik-Medium";
  font-size: 25px;
  line-height: 30px;
  letter-spacing: 0em;
  text-align: left;
  margin-bottom: 3rem;
}

.section__toolkit h3 {
  font-weight: 900;
  font-family: "Graphik-Medium";
  font-size: 21px;
  line-height: 30px;
  letter-spacing: 0em;
  text-align: left;
  margin-bottom: 3rem;
}

.section-design__toolkit {
  display: flex;
  justify-content: space-between;
  width: 30rem;
}

.design__methods li {
  margin: 30px 0;
  list-style: none;
  font-family: "Graphik-Regular";
  font-size: 19px;
  font-weight: 400;
  line-height: 40px;
  letter-spacing: 0em;
  text-align: left;
}

.design__methods li span {
  margin-right: 20px;
}

.design__tools li {
  margin: 30px 0;
  list-style: none;
  font-family: "Graphik-Regular";
  font-size: 19px;
  font-weight: 400;
  line-height: 40px;
  letter-spacing: 0em;
  text-align: left;
}

.design__tools li span {
  margin-right: 20px;
}

.section-work__history h2 {
  font-weight: 900;
  font-family: "Graphik-Medium";
  font-size: 25px;
  line-height: 30px;
  letter-spacing: 0em;
  text-align: left;
  margin-bottom: 3rem;
}

.section__history {
  display: flex;
}

.work__history {
  width: 15rem;
}

.work__history li {
  list-style: none;
  font-weight: 900;
  font-family: "Graphik-Medium";
  font-size: 19px;
  line-height: 40px;
  letter-spacing: 0em;
  text-align: left;
}

.work__history li span {
  margin-right: 20px;
}

.parkway-projects-work__history li {
  list-style: none;
  font-weight: 900;
  font-family: "Graphik-Medium";
  font-size: 19px;
  line-height: 40px;
  letter-spacing: 0em;
  text-align: left;
}

.parkway-projects-work__history span {
  margin-right: 20px;
}

.role {
  font-family: "Graphik-Regular";
  font-size: 16px;
  font-weight: 300;
  line-height: 30px;
  letter-spacing: 0em;
  text-align: left;
  margin-top: 1rem;
  margin-bottom: 1rem;
}

.time {
  font-family: "Graphik-Regular";
  font-size: 16px;
  font-weight: 300;
  line-height: 30px;
  letter-spacing: 0em;
  text-align: left;
  margin-top: 1rem;
  margin-bottom: 2rem;
  border: 1px solid #000;
  width: 150px;
  padding: 2px 20px;
  border-radius: 20px;
}

.section-interest__container {
  padding-top: 5rem;
  padding-bottom: 7rem;
  max-width: 109.2rem;
  margin: 0 auto;
  padding-left: 121px;
  padding-right: 121px;
  display: flex;
  justify-content: space-between;
}

.section-interest__reading h3 {
  font-weight: 900;
  font-family: "Graphik-Medium";
  font-size: 20px;
  line-height: 30px;
  letter-spacing: 0em;
  text-align: left;
  margin-bottom: 2rem;
}

.section-interest__reading img {
  max-width: 70px;
  margin-right: 20px;
}

.section-interest__listening h3 {
  font-weight: 900;
  font-family: "Graphik-Medium";
  font-size: 20px;
  line-height: 30px;
  letter-spacing: 0em;
  text-align: left;
  margin-bottom: 2rem;
}

.section-interest__listening h6 {
  font-family: "Graphik-Regular";
  font-size: 18px;
  font-weight: 500;
  line-height: 30px;
  letter-spacing: 0em;
  text-align: left;
  margin-bottom: 2rem;
}

.section-interest__listening img {
  max-width: 70px;
  margin-right: 20px;
}

.section-interest__listening__music h6 {
  font-family: "Graphik-Regular";
  font-size: 18px;
  font-weight: 500;
  line-height: 30px;
  letter-spacing: 0em;
  text-align: left;
  margin-top: 2rem;
  margin-bottom: 2rem;
}

@media screen and (min-width: 1600px) {
  .about-text__container {
    width: 50rem;
  }
}

@media screen and (max-width: 1300px) {
  /* .about__container {
    flex-direction: column;
  } */
  .hero__image {
    /* width: 800px; */
  }

  .about-text__container {
    width: 40rem;
  }

  .section__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .section-interest__reading img {
    margin-bottom: 4rem;
  }
}

@media screen and (max-width: 980px) {
  .about__container {
    padding: 7rem 64px;
    flex-direction: column;
  }

  .hero__image {
    /* width: 600px; */
  }

  .section__container {
    flex-direction: column;
  }

  .section__toolkit {
    margin-bottom: 4rem;
  }

  .section-interest__container {
    padding-left: 64px;
    padding-right: 64px;
    flex-direction: column;
  }
}

@media screen and (max-width: 768px) {
  .about__container {
    padding-left: 24px;
    padding-right: 24px;
  }

  .hero__image {
    width: 100%;
  }

  .about-text__container {
    width: 100%;
  }

  .section__container {
    padding-left: 24px;
    padding-right: 24px;
  }

  .section-design__toolkit {
    flex-direction: column;
    width: 100%;
  }

  .section__history {
    flex-direction: column;
  }

  .design__methods {
    margin-bottom: 4rem;
  }

  .section-interest__container {
    padding-left: 24px;
    padding-right: 24px;
  }
}

@media screen and (max-width: 540px) {
  .landing__page {
  background-image: url("../assets/images/lines-for-mobile.svg");
  background-position: top center;
}

  .about__header {
    font-size: 26px !important;
    font-weight: 300 !important;
  }

  .contact__container h3 {
    font-size: 22px;
    font-weight: 200;
  }

  .about-text__container p {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }

  .section__toolkit h2 {
    font-weight: 300;
    font-size: 24px;
  }

  .section__toolkit h3 {
    font-weight: 600;
    font-size: 18px;
    line-height: 30px;
  }

  .design__methods li {
    font-size: 16px;
    font-weight: 300;
    line-height: 40px;
  }

  .design__tools li {
    font-size: 16px;
    font-weight: 300;
    line-height: 40px;
  }

  .section-work__history h2 {
    font-weight: 300;
    font-size: 24px;
  }

  .section-interest__reading h3 {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }

  .section-interest__listening h3 {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }

  .section-interest__listening h6 {
    font-size: 16px;
    font-weight: 300;
    line-height: 40px;
  }

  .section-interest__listening__music h6 {
    font-size: 16px;
    font-weight: 300;
    line-height: 40px;
  }
}
</style>

<template>
  <div>
    <Header></Header>
    <article class="product__container">
      <article class="product__header">
        <p>Coded Agents Redesign</p>
      </article>

      <article class="product__text">
        <p>
          Coded Agents is a mobile app that helps connects Home Agents to people
          <br />
          who are looking for homes to buy or rent for a perod of time.
        </p>
      </article>

      <article class="role-description__container">
        <p>2021</p>
        <p>Type - Housing</p>
        <p>Role - Product Designer</p>
        <p>Platform - Mobile Application, Website</p>
      </article>
    </article>

    <section class="coded-agents-hero__image">
      <img
        src="../assets/images/coded-agents-hero-image.png"
        alt=""
        width="100%"
      />
    </section>

    <section class="about-product__container">
      <section class="product__brief">
        <p class="product__brief__header">Brief</p>
        <p class="product__brief__text">
          Housing is one of the issues that people have had a hard time to find
          a solution to, and this is where coded agents comes in. A lot of
          housing agents have houses for rent, short let or sale and have no
          place to upload information about these houses to prospective tenants
          or their fellow agents except with the use of social media. Coded
          Agents provides a community where you can upload all the information
          of the property on the platform and even sell it there without having
          to leave the platform or post on social media.
        </p>
      </section>

      <section class="product__challenge">
        <p class="product__challenge__header">The challenge</p>
        <div class="product__challenge__text">
          <ul class="product__challenge__list">
            <li style="padding-left: 1em">
              Redesigning the existing app into something that is easier to use
              and more visually appealing.
            </li>

            <li style="padding-left: 1em">
              Making the flow much more easier and transparent than what was
              already existing therefore increasing more user sign ups and more
              house sales.
            </li>
          </ul>
        </div>
      </section>
      <section class="product__role">
        <p class="product__role__header">My Role & the team</p>
        <p class="product__role__text">
          I worked in a design team of three here as the lead product designer on this product, I spear headed product design efforts which included reworking the sign up flow, sale flow and choosing new color schemes to use on the product.
        </p>
      </section>

      <section class="research__container">
        <p class="research__header">Research & User Experience</p>
        <p class="research__text">
          For this product we realised agents weren’t utilizing it properly and will rather use social media to pass accross their information, so we were able to ask quite a number of agents that had signed up on the existing app why they weren’t using it and also asked agents who hadn’t signed up what they want to see in a product like this. This is how some of the interviews went :
        </p>
      </section>
    </section>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
export default {
  components: Header,
};
</script>

<style scoped>
.product__container {
  flex-direction: column;
  max-width: 109.2rem;
  margin: 0 auto;
  padding-top: 7rem;
  padding-bottom: 5rem;
  padding-left: 128px;
  padding-right: 128px;
}

.product__header {
  font-family: "Graphik-SemiBold";
  font-size: 2rem;
  font-weight: 600;
  /* letter-spacing: 0.02em; */
  line-height: 4.5rem;
  max-width: 55rem;
}

.product__text {
  font-family: "Graphik-Regular";
  font-size: 1.3rem;
  font-weight: 300;
  line-height: 3rem;
  max-width: 54rem;
}

.role-description__container {
  display: flex;
}

.role-description__container p {
  font-family: "Graphik-Regular";
  font-size: 16px;
  font-weight: 300;
  line-height: 30px;
  letter-spacing: 0em;
  text-align: left;
  margin-top: 2rem;
  margin-bottom: 2rem;
  border: 1px solid #000;
  padding: 2.5px 20px;
  border-radius: 20px;
  margin-right: 20px;
}

.role-description__container p:nth-child(1) {
  padding: 2.5px 35px;
}

.coded-agents-hero__image {
  padding: 0 128px;
  max-width: 109.2rem;
  margin: 0 auto;
}

.coded-agents-hero__image img {
  width: 100%;
}

.about-product__container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  max-width: 109.2rem;
  margin: 0 auto;
  padding-bottom: 5rem;
  padding-left: 128px;
  padding-right: 128px;
}

.product__brief {
  margin-top: 6rem;
  margin-bottom: 2rem;
}

.product__brief__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.product__brief__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 3rem;
}

.product__challenge {
  margin-top: 3rem;
  margin-bottom: 2rem;
}

.product__challenge__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.product__challenge__list {
  list-style-image: url("~assets/images/Polygon.png");
}

.product__challenge__list li {
  margin-left: 20px;
  padding: 20px 0;
  font-family: "Graphik-Regular";
  font-size: 19px;
  font-weight: 400;
  line-height: 40px;
  letter-spacing: 0em;
  text-align: left;
}

.product__role {
  margin-top: 3rem;
  margin-bottom: 2rem;
}

.product__role__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.product__role__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 3rem;
}

.product__role__text span {
  font-weight: 900;
  font-family: "Graphik-Medium";
}

.research__container {
  margin-top: 3rem;
  margin-bottom: 2rem;
}

.research__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.research__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 3rem;
}
</style>

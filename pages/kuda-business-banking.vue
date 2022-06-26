<template>
  <div>
    <Header></Header>
    <article class="product__container">
      <article class="product__header">
        <p>Kuda Business Banking</p>
      </article>

      <article class="product__text">
        <p>
          A digital business bank that helps business users make payments,<br />
          create invoices and also manage multiple accounts seamlessly.
        </p>
      </article>

      <article class="role-description__container">
        <p>2021 - Present</p>
        <p>Type - Fintech</p>
        <p>Role - Product Designer</p>
        <p>Platform - Web Application, Mobile Application</p>
      </article>
    </article>

    <section class="kuda-hero__image">
      <img src="../assets/images/kuda-hero-image.png" alt="" width="100%" />
    </section>

    <section class="about-product__container">
      <section class="product__brief">
        <p class="product__brief__header">Brief</p>
        <p class="product__brief__text">
          Everyday new businesses are formed, whether petty businesses (sole
          trader) or large scale businesses and a lot of business owners like to
          separate their personal earnings from that of the business hence they
          open new bank accounts for the business and with a product like Kuda
          Business, the goal was to build a business product that satisfies all
          the banking needs of a business i.e being able to receive and send
          money, create/seend invoices and also pay bills.
        </p>
      </section>

      <section class="product__challenge">
        <p class="product__challenge__header">The challenge</p>
        <div class="product__challenge__text">
          <ul class="product__challenge__list">
            <li style="padding-left: 1em">
              Provide a solution for business owners with petty businesses that
              aren’t registered
            </li>

            <li style="padding-left: 1em">
              Allow users to be able to track their activities on their business
              account i.e inflow, outflow
            </li>

            <li style="padding-left: 1em">
              Provide a solution that allows business owners to send and receive
              money seamlessly and also pay bills.
            </li>

            <li style="padding-left: 1em">
              Provide a solution that allows business owners to send out
              invoices to their customers and be paid directly.
            </li>
          </ul>
        </div>
      </section>

      <section class="product__role">
        <p class="product__role__header">My Role & the team</p>
        <p class="product__role__text">
          On this product I worked as a product designer on a large team of
          product designers, product managers and developers.
        </p>

        <p class="sub-product__role__header">Collaborators</p>
        <p class="sub-product__role__text">
          <span>Derek Kanu,</span> <span>Tunde Mason,</span>
          <span>Okoronkwo Kanno,</span> <span>Omono Etomi,</span>
          <span>Michael Abegunde,</span> <span>Paul Adedokun</span>
        </p>
      </section>

      <section class="product-target__audience">
        <p class="product-target__audience__header">Target Audience</p>
        <p class="product-target__audience__text">
          Our target audience for this product consists of business owners i.e
          with petty businesses and registered businesses.
        </p>
      </section>

      <section class="product__solution">
        <p class="product__solution__header">The Solution</p>
        <p class="product__solution__text">
          After the team had gathered the information neccessary, the next step
          was to work on the user journey hand in hand with the PRD (Product
          Requirement Documents) given by the product managers, this step helps
          in streamlining the things the users want to see in the product.
        </p>
      </section>
    </section>

    <section class="flow-chart__container">
      <section class="flow-chart-onboarding__container">
        <section class="flow-chart-onboarding__content">
          <section class="flow-chart-onboarding__images">
            <img
              src="../assets/images/Kuda Business Onboarding V2-New-to-Bank Onboarding final.png"
              alt=""
            />
          </section>
        </section>
      </section>
      <p class="flow-chart-onboarding__image__caption">Onboarding Flow</p>

      <section class="business-registration__container">
        <section class="business-registration__content">
          <section class="business-registration__images">
            <img
              src="../assets/images/Kuda Business Onboarding V2-Business Registration.png"
              alt=""
            />
          </section>
        </section>
      </section>
      <p class="business-registration__image__caption">Business registration</p>
    </section>

    <section class="visual-design__container">
      <p class="visual-design__header">Visual Design</p>
      <p class="visual-design__sub__header">Style guide</p>
      <p class="visual-design__text">
        Below we have the style guide used to work on the visual design for this
        product, from the colors (primary & secondary) to the font family,
        buttons and icons used.
        <span>NB : Primary colors #FFFFF, #0A0411 and Font family Mulish.</span>
      </p>

      <section class="visual-design__image__container">
        <img src="../assets/images/kuda-color.png" alt="" />
        <img src="../assets/images/kuda-typography.png" alt="" />
        <img src="../assets/images/kuda-button-components.png" alt="" />
        <img src="../assets/images/kuda-icon-components.png" alt="" />
      </section>
    </section>

    <section class="onboarding__container">
      <p class="onboarding__header">Onboarding</p>
      <p class="onboarding__text">
        For our onboarding process on this product, there are two options, the
        user can either choose to sign up as a new user or sign up with their
        existing <span>Kuda "Retail" account,</span> the reason for the first
        option is for people who do not have existing Kuda Retail accounts.
      </p>
    </section>

    <section class="onboarding-hero__image">
      <img src="../assets/images/kuda-onboarding-image.png" alt="" />
    </section>

    <InputingYourDetailsGallery></InputingYourDetailsGallery>
    <SendingMoneyGallery></SendingMoneyGallery>
    <InvoicingGallery></InvoicingGallery>

    <section class="mobile-screens__container">
      <p class="mobile-screens__header">Mobile Screens</p>
      <p class="mobile-screens__text">
        These are some screens from the mobile app.
      </p>
    </section>
    <!-- <section class="mobile-screens__images__container">
      <section class="mobile-screens__images">
        <img src="../assets/images/welcome-screen-2.png" alt="" />
        <img src="../assets/images/welcome-screen-3.png" alt="" />
        <img src="../assets/images/welcome-screen-4.png" alt="" />
      </section>
    </section>-->
    <!-- <img
      src="../assets/images/mobile-screens-background.png"
      alt=""
      class="mobile-screens__backhround__image"
    /> -->
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import SendingMoneyGallery from "../components/sending-money-gallery.vue";
import InvoicingGallery from "../components/invoicing-gallery.vue";
import InputingYourDetailsGallery from "../components/inputing-your-details-gallery.vue";
export default {
  data() {
    return {};
  },

  components: {
    Header,
    SendingMoneyGallery,
    InvoicingGallery,
    InputingYourDetailsGallery,
  },
};
</script>

<style scoped>
.product__container {
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

.product__header {
  font-family: "Graphik-SemiBold";
  font-size: 2rem;
  font-weight: 600;
  /* letter-spacing: 0.02em; */
  line-height: 4.5rem;
  margin-bottom: 1.8rem;
  max-width: 55rem;
}

.product__text {
  font-family: "Graphik-Regular";
  font-size: 1.3rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 1rem;
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

.kuda-hero__image {
  padding: 0 128px;
  max-width: 109.2rem;
  margin: 0 auto;
}

.kuda-hero__image img {
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

.sub-product__role__header {
  font-family: "Graphik-Medium";
  font-size: 1.3rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.sub-product__role__text {
  font-family: "Graphik-Regular";
  font-size: 1rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 3rem;
}

.sub-product__role__text span {
  text-decoration: underline;
}

.product-target__audience {
  margin-top: 2rem;
  margin-bottom: 2rem;
}

.product-target__audience__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.product-target__audience__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 3rem;
}

.product__solution {
  margin-top: 2rem;
  margin-bottom: 1rem;
}

.product__solution__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.product__solution__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  /* margin-bottom: 1rem; */
}

.flow-chart__container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  max-width: 109.2rem;
  margin: 0 auto;
  /* padding-top: 1rem; */
  padding-bottom: 7rem;
}

.flow-chart-onboarding__container {
  background: #f0f8fb;
  padding: 64px 0;
  margin: 3rem 128px;
}

.flow-chart-onboarding__content {
  max-width: 109.2rem;
  margin: 0 auto;
  padding-left: 32px;
  padding-right: 32px;
}

.flow-chart-onboarding__images img {
  width: 100%;
  margin: 0 auto;
}

.flow-chart-onboarding__image__caption {
  font-family: "Graphik-Regular";
  font-size: 1.3rem;
  font-weight: 300;
  text-align: center;
}

.business-registration__container {
  background: #f0f8fb;
  padding: 64px 0;
  margin: 3rem 128px;
}

.business-registration__content {
  max-width: 109.2rem;
  margin: 0 auto;
  padding-left: 32px;
  padding-right: 32px;
}

.business-registration__images img {
  width: 100%;
  margin: 0 auto;
}

.business-registration__image__caption {
  font-family: "Graphik-Regular";
  font-size: 1.3rem;
  font-weight: 300;
  text-align: center;
}

.visual-design__container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  max-width: 109.2rem;
  margin: 0 auto;
  padding-top: 2rem;
  padding-bottom: 7rem;
  padding-left: 128px;
  padding-right: 128px;
}

.visual-design__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 3rem;
}

.visual-design__sub__header {
  font-family: "Graphik-Medium";
  font-size: 1.3rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.visual-design__text {
  font-family: "Graphik-Regular";
  font-size: 1.3rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 1rem;
}

.visual-design__text span {
  font-weight: 900;
  font-family: "Graphik-Medium";
}

.visual-design__image__container {
  display: flex;
  flex-wrap: wrap;
}

.visual-design__image__container img {
  width: 396px;
  padding-top: 5rem;
}

.visual-design__image__container img:nth-child(1) {
  margin-right: 231px;
}

.visual-design__image__container img:nth-child(3) {
  margin-right: 231px;
  max-height: 880px;
}

.onboarding__container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  max-width: 109.2rem;
  margin: 0 auto;
  padding-top: 2rem;
  padding-bottom: 5rem;
  padding-left: 128px;
  padding-right: 128px;
}

.onboarding__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.onboarding__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 3rem;
}

.onboarding__text span {
  font-weight: 900;
  font-family: "Graphik-Medium";
}

.onboarding-hero__image {
  padding: 0 128px;
  max-width: 109.2rem;
  margin: 0 auto;
}

.onboarding-hero__image img {
  width: 100%;
}

.mobile-screens__container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  max-width: 109.2rem;
  margin: 0 auto;
  padding-top: 7rem;
  padding-bottom: 7rem;
  padding-left: 128px;
  padding-right: 128px;
}

.mobile-screens__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.mobile-screens__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 3rem;
}

/* .mobile-screens__images__container {
  max-width: 109.2rem;
  margin: 0 auto;
  padding-left: 128px;
  padding-right: 128px;
}

.mobile-screens__images img {
  width: 375px;
  z-index: 7;
}

.mobile-screens__backhround__image {
  width: 1345px;
  height: 592px;
  margin: 0 47px;
  position: relative;
  top: 13303px;
} */

@media screen and (max-width: 1240px) {
  .role-description__container {
    flex-wrap: wrap;
  }

  .role-description__container p {
    margin-bottom: 0.5rem;
  }
}

@media screen and (max-width: 980px) {
  .product__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .about-product__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .kuda-hero__image {
    padding: 0 64px;
  }

  .flow-chart-onboarding__container {
    margin: 3rem 64px;
  }

  .business-registration__container {
    margin: 3rem 64px;
  }

  .visual-design__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .visual-design__image__container img {
    width: 100%;
    /* padding-top: 5rem; */
  }

  /* .visual-design__image__container img:nth-child(3) {
    margin-right: 231px;
    max-height: 880px;
  } */

  .onboarding__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .onboarding-hero__image {
    padding: 0 64px;
  }
}

@media screen and (max-width: 768px) {
  .product__container {
    padding-left: 32px;
    padding-right: 32px;
  }

  .about-product__container {
    padding-left: 32px;
    padding-right: 32px;
  }

  .kuda-hero__image {
    padding: 0 32px;
  }

  .flow-chart-onboarding__container {
    margin: 3rem 32px;
  }

  .business-registration__container {
    margin: 3rem 32px;
  }

  .visual-design__container {
    padding-left: 32px;
    padding-right: 32px;
  }

  .onboarding__container {
    padding-left: 32px;
    padding-right: 32px;
  }

  .onboarding-hero__image {
    padding: 0 32px;
  }
}

@media screen and (max-width: 540px) {
  .product__header {
    font-size: 26px;
    font-weight: 300;
    line-height: 50px;
  }

  .product__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }

  .role-description__container p {
    font-size: 16px;
  }

  .product__brief__header {
    font-size: 26px;
    font-weight: 300;
  }

  .product__brief__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }

  .product__challenge__header {
    font-size: 26px;
    font-weight: 300;
  }

  /* .product__challenge__list li {
    margin-left: 20px;
    padding: 20px 0;
    font-family: "Graphik-Regular";
    font-size: 19px;
    font-weight: 400;
    line-height: 40px;
    letter-spacing: 0em;
    text-align: left;
  } */

  .product__role__header {
    font-size: 26px;
    font-weight: 300;
  }

  .product__role__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }

  .sub-product__role__header {
    font-size: 26px;
    font-weight: 300;
  }

  .sub-product__role__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }

  /* .sub-product__role__text span {
    text-decoration: underline;
  } */

  .product-target__audience {
    margin-top: 2rem;
    margin-bottom: 2rem;
  }

  .product-target__audience__header {
    font-size: 26px;
    font-weight: 300;
  }

  .product-target__audience__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }

  .product__solution {
    margin-top: 2rem;
    margin-bottom: 1rem;
  }

  .product__solution__header {
    font-size: 26px;
    font-weight: 300;
  }

  .product__solution__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }
}
</style>

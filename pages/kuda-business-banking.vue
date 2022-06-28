<template>
  <div>
    <Header></Header>
    <article class="product__container">
      <article class="product__header">
        <p>Kuda Business Banking</p>
      </article>

      <article class="product__text">
        <p>
          A digital business bank that helps business users make payments,
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
      <img
        src="../assets/images/kuda-hero-image.png"
        alt=""
        class="hero-image"
        width="100%"
      />
      <img
        src="../assets/images/kuda-mobile-image.png"
        class="mobile-image"
        alt=""
        width="100%"
      />
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
    <section class="mobile-screens-one__images">
      <img src="../assets/images/welcome-screen-2.png" alt="" />
      <img src="../assets/images/welcome-screen-3.png" alt="" />
      <img src="../assets/images/welcome-screen-4.png" alt="" />
    </section>

    <section class="mobile-screens-two__images">
      <img src="../assets/images/landing-page-signed-in.png" alt="" />
      <img src="../assets/images/personal-details.png" alt="" />
      <img src="../assets/images/verify-ID-first-step.png" alt="" />
    </section>

    <section class="mobile-screens-three__images">
      <img src="../assets/images/bank.png" alt="" />
      <img src="../assets/images/invoice.png" alt="" />
      <img src="../assets/images/get-started.png" alt="" />
    </section>

    <section class="product__challenge__and__takeaway">
      <p class="product__challenges__header">Challenges and Takeaways</p>
      <p class="product__challenges__text">
        This project provided an excellent opportunity to learn about designing
        for security and ease, a business owner won’t want to keep their money
        in your bank if they aren’t sure their money is safe and easily
        accessible whenever they need it, so we had to put that into
        consideration when designing and optimize for accessibility and easy
        usage.
      </p>
    </section>

    <section class="product__conclusion">
      <p class="product__conclusion__header">Conclusion and Outcome</p>
      <p class="product__conclusion__text">
        Kuda Business is a product under Kuda MFB which has over 3 million
        customers and is currently in it’s expansion phase to the UK and other
        African country, Kuda Business since it’s launch has helped add to the
        total Kuda MFB users with over 100,000 customers here in Lagos, Nigeria.
        As we continue growing more features will be added to satisfy out large
        and ever increasing customer base.
      </p>
    </section>

    <section class="product-CTA_link">
      <p>
        <a href="https://kuda.com/business/">Click here to go to website</a>
      </p>
    </section>

    <section class="product__footer">
      <p class="product__presentation">Presentation available on request</p>
      <section class="product__next__container">
        <p class="product__next__header">Next Project</p>
        <p class="product__next__text">
          <Nuxt-Link to="/monthly">Monthly</Nuxt-Link>
        </p>
      </section>
    </section>
    <SubFooter></SubFooter>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import SendingMoneyGallery from "../components/sending-money-gallery.vue";
import InvoicingGallery from "../components/invoicing-gallery.vue";
import InputingYourDetailsGallery from "../components/inputing-your-details-gallery.vue";
import SubFooter from "../components/SubFooter.vue";
export default {
  data() {
    return {};
  },

  components: {
    Header,
    SendingMoneyGallery,
    InvoicingGallery,
    InputingYourDetailsGallery,
    SubFooter,
  },
};
</script>

<style scoped>
.product__container {
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

.mobile-image {
  display: none;
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
}

.flow-chart__container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  max-width: 109.2rem;
  margin: 0 auto;
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
  /* display: flex;
  flex-direction: column;
  justify-content: space-between; */
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

.mobile-screens-one__images {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 64px;
  padding: 0 96px;
  background: url("../assets/images/mobile-screens-background.png");
  background-repeat: no-repeat;
  background-size: 100% 592px;
  background-position: bottom;
  margin-left: 47px;
  margin-right: 47px;
  margin-bottom: 200px;
}

.mobile-screens-one__images img {
  max-width: 375px;
  max-height: 812px;
  position: relative;
  top: -73px;
}

.mobile-screens-two__images {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 64px;
  padding: 0 96px;
  background: url("../assets/images/mobile-screens-background.png");
  background-repeat: no-repeat;
  background-size: 100% 592px;
  background-position: bottom;
  margin-left: 47px;
  margin-right: 47px;
  margin-bottom: 200px;
}

.mobile-screens-two__images img {
  max-width: 375px;
  height: 812px;
  position: relative;
  top: -73px;
}

.mobile-screens-two__images img:nth-child(2) {
  height: 877px;
  top: -41px;
}

.mobile-screens-two__images img:nth-child(3) {
  height: 845px;
  top: -58px;
}

.mobile-screens-three__images {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 64px;
  padding: 0 96px;
  background: url("../assets/images/mobile-screens-background.png");
  background-repeat: no-repeat;
  background-size: 100% 592px;
  background-position: bottom;
  margin-left: 47px;
  margin-right: 47px;
  margin-bottom: 200px;
}

.mobile-screens-three__images img {
  max-width: 375px;
  max-height: 812px;
  position: relative;
  top: -73px;
}

.mobile-screens-three__images img:nth-child(1) {
  height: 882px;
  top: -68px;
}

.product__challenge__and__takeaway {
  max-width: 109.2rem;
  margin: 0 auto;
  padding-bottom: 5rem;
  padding-left: 128px;
  padding-right: 128px;
}

.product__challenges__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.product__challenges__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 1rem;
}

.product__conclusion {
  max-width: 109.2rem;
  margin: 0 auto;
  padding-bottom: 3rem;
  padding-left: 128px;
  padding-right: 128px;
}

.product__conclusion__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.product__conclusion__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 1rem;
}

.product-CTA_link {
  max-width: 109.2rem;
  margin: 0 auto;
  padding-bottom: 5rem;
  padding-left: 128px;
  padding-right: 128px;
}

.product-CTA_link p a {
  font-family: "Graphik-Medium";
  font-size: 18px;
  font-weight: 500;
  line-height: 33px;
  color: #14586d;
  text-align: left;
  text-decoration: none;
}

.product__footer {
  max-width: 109.2rem;
  margin: 0 auto;
  padding-bottom: 5rem;
  padding-left: 128px;
  padding-right: 128px;
}

.product__presentation {
  font-family: "Graphik-SemiBold";
  font-size: 26px;
  font-weight: 600;
  line-height: 30px;
  text-align: center;
  margin-top: 69px;
  color: #14586d;
}

.product__next__container {
  margin-top: 150px;
  margin-bottom: 118px;
  text-align: center;
}

.product__next__header {
  font-family: "Graphik-SemiBold";
  font-size: 25px;
  font-weight: 600;
  line-height: 30px;
  margin-bottom: 17px;
}

.product__next__text a {
  font-family: "Graphik-SemiBold";
  font-size: 16px;
  font-weight: 400;
  line-height: 30px;
  color: #979797;
  text-decoration: none;
}

/* .nav__items__center a:active,
.nav__items__center a.nuxt-link-active {
  border-bottom: 3px solid #14586d;
} */

@media screen and (max-width: 1240px) {
  .role-description__container {
    flex-wrap: wrap;
  }

  .role-description__container p {
    margin-bottom: 0.5rem;
  }

  .mobile-screens-one__images {
    flex-direction: column;
    background-size: 100% 2000px;
    margin-left: 0;
    margin-right: 0;
    margin-bottom: 250px;
  }

  .mobile-screens-two__images {
    flex-direction: column;
    background-size: 100% 2000px;
    margin-left: 0;
    margin-right: 0;
    margin-bottom: 250px;
  }

  .mobile-screens-three__images {
    flex-direction: column;
    background-size: 100% 2000px;
    margin-left: 0;
    margin-right: 0;
    margin-bottom: 250px;
  }

  .mobile-screens-one__images img {
    top: 0;
  }

  .mobile-screens-two__images img {
    top: 0;
  }

  .mobile-screens-three__images img {
    top: 0;
  }

  .mobile-screens-two__images img:nth-child(2) {
    top: 0;
  }

  .mobile-screens-two__images img:nth-child(3) {
    top: 0;
  }

  .mobile-screens-three__images img:nth-child(1) {
    top: 0;
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
  }

  .onboarding__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .onboarding-hero__image {
    padding: 0 64px;
  }

  .mobile-screens__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .product__challenge__and__takeaway {
    padding-left: 64px;
    padding-right: 64px;
  }

  .product__conclusion {
    padding-left: 64px;
    padding-right: 64px;
  }

  .product-CTA_link {
    padding-left: 64px;
    padding-right: 64px;
  }

  .product__footer {
    padding-left: 64px;
    padding-right: 64px;
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

  .mobile-screens__container {
    padding-left: 32px;
    padding-right: 32px;
  }

  .product__challenge__and__takeaway {
    padding-left: 32px;
    padding-right: 32px;
  }

  .product__conclusion {
    padding-left: 32px;
    padding-right: 32px;
  }

  .product-CTA_link {
    padding-left: 32px;
    padding-right: 32px;
  }

  .product__footer {
    padding-left: 32px;
    padding-right: 32px;
  }
}

@media screen and (max-width: 540px) {
  .product__container {
    padding-top: 41px;
  }

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

  .hero-image {
    display: none;
  }

  .mobile-image {
    display: block;
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

  .visual-design__header {
    font-size: 26px;
    font-weight: 300;
  }

  .visual-design__sub__header {
    font-size: 18px;
    font-weight: 300;
  }

  .visual-design__text {
    font-size: 18px;
    font-weight: 300;
  }

  .onboarding__header {
    font-size: 26px;
    font-weight: 300;
    line-height: 50px;
  }

  .onboarding__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 43px;
  }

  .product__challenges__header {
    font-size: 26px;
    font-weight: 300;
    line-height: 50px;
  }

  .product__challenges__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }

  .product__conclusion__header {
    font-size: 26px;
    font-weight: 300;
    line-height: 50px;
  }

  .product__conclusion__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }

  .product-CTA_link p a {
    font-size: 16px;
    font-weight: 300;
  }

  .product__presentation {
    font-size: 22px;
    font-weight: 300;
    line-height: 40px;
  }

  .product__next__header {
    font-size: 25px;
    font-weight: 300;
    line-height: 30px;
  }

  .product__next__text a {
    font-size: 16px;
    font-weight: 300;
    line-height: 30px;
  }
}

@media screen and (max-width: 375px) {

}
</style>

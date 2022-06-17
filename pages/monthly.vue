<template>
  <div>
    <Header></Header>
    <article class="product__container">
      <article class="product__header">
        <p>Monthly</p>
      </article>

      <article class="product__text">
        <p>
          Monthly is a product that allows people take rent loans, and pay it
          <br />
          back monthly, so as to help their financial freedom and flexibility.
        </p>
      </article>

      <article class="role-description__container">
        <p>2022</p>
        <p>Type - Fintech</p>
        <p>Role - Product Designer</p>
        <p>Platform - Mobile Application, Website</p>
      </article>
    </article>

    <section class="monthly-hero__image">
      <img src="../assets/images/monthly-hero-image.png" alt="" width="100%" />
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
          <div class="product__challenge__list">
            <p>
              <span><img src="../assets/images/Polygon.png" alt="" /></span>How
              do we build a usable product that solves the issue of yearly
              payment of rent by the tenant and make life easier for them.
            </p>

            <p>
              <span><img src="../assets/images/Polygon.png" alt="" /></span>How
              do we validate the tenants financial background so we will know if
              they have the ability to pay back their loans
            </p>

            <p>
              <span><img src="../assets/images/Polygon.png" alt="" /></span>How
              do we build a seamless platform where it is easy for the tenant to
              pay back loans
            </p>
          </div>
        </div>
      </section>

      <section class="product__role">
        <p class="product__role__header">My Role & the team</p>
        <p class="product__role__text">
          I was strictly in charge of the product design work on this product,
          for the mobile apps (iOS & Android) and the marketing website, I
          worked in a design team of 2 people where I led the product design
          efforts and the second person <span>Adeniyi Oyenaike</span> led the
          graphic design (logo, icons packs etc) efforts.
        </p>
      </section>

      <section class="research__container">
        <p class="research__header">Research & User Experience</p>
        <p class="research__text">
          We got the incentive to build Monthly after seeing a number of people
          on Twitter complain about how ridiculous it is that they have to pay a
          full years rent before being able to move into an apartment, a poll
          was conducted and we realized that 72% of people do not have up to the
          amount to pay a full year down payment, while 26% have that amount but
          they’d rather not and they prefer a payment plan approach, the
          remaining 2% were fine with paying for everything at once.
        </p>
      </section>
    </section>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
export default {
  components: {
    Header,
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
  font-family: "Graphik-Bold";
  font-size: 2rem;
  font-weight: 900;
  letter-spacing: 0.02em;
  line-height: 4.5rem;
  /* margin-bottom: 1.5rem; */
  max-width: 55rem;
}

.product__text {
  font-family: "Graphik-Regular";
  font-size: 1.3rem;
  font-weight: 300;
  line-height: 3rem;
  /* margin-bottom: 1rem; */
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
  margin-top: 1rem;
  margin-bottom: 2rem;
  border: 1px solid #000;
  padding: 2.5px 20px;
  border-radius: 20px;
  margin-right: 20px;
}

.role-description__container p:nth-child(1) {
  padding: 2.5px 35px;
}

.monthly-hero__image {
  padding: 0 128px;
  max-width: 109.2rem;
  margin: 0 auto;
}

.monthly-hero__image img {
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
  margin-top: 7rem;
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

.product__challenge__list p {
  margin: 30px 0;
  /* list-style: none; */
  font-family: "Graphik-Regular";
  font-size: 19px;
  font-weight: 400;
  line-height: 40px;
  letter-spacing: 0em;
  text-align: left;
}

.product__challenge__list p span {
  margin-right: 20px;
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

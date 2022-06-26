<template>
  <div>
    <Header></Header>

    <section class="more-designs__container">
      <p class="more-designs__header">More Designs</p>
      <p class="more-designs__text">
        These are some of my other commissioned design works, consisting of
        mobile and web designs.
      </p>

      <section class="design__images">
        <div class="design__container">
          <img src="../assets/images/design-1.png" alt="" />
          <p class="design__caption">MAX Delivery Admin Dashboard</p>
        </div>
        <div class="design__container">
          <img src="../assets/images/design-2.png" alt="" />
          <p class="design__caption">Megalectrics Radio App</p>
        </div>
        <div class="design__container">
          <img src="../assets/images/design-3.png" alt="" />
          <p class="design__caption">MAX Delivery Driver Web App</p>
        </div>
        <div class="design__container">
          <img src="../assets/images/design-4.png" alt="" />
          <p class="design__caption">Fieldinsight website</p>
        </div>
      </section>
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
.more-designs__container {
  max-width: 109.2rem;
  margin: 0 auto;
  padding-top: 7rem;
  padding-bottom: 5rem;
  padding-left: 128px;
  padding-right: 128px;
}

.more-designs__header {
  font-family: "Graphik-SemiBold";
  font-size: 2rem;
  font-weight: 600;
  /* letter-spacing: -0.03em; */
  line-height: 4.5rem;
  margin-bottom: 1.5rem;
}

.more-designs__text {
  font-family: "Graphik-Regular";
  font-size: 1.3rem;
  font-weight: 300;
  line-height: 3rem;
}

.design__images {
  display: flex;
  flex-wrap: wrap;
  gap: 75px;
  margin-top: 5rem;
  margin-bottom: 8rem;
}

.design__images img {
  max-width: 550px;
}

.design__caption {
  font-family: "Graphik-Regular";
  margin-top: 1rem;
  font-size: 18px;
  font-weight: 900;
}

@media screen and (min-width: 1600px) {
  .design__images {
    gap: 50px;
  }

  .design__images img {
    max-width: 718px;
  }
}

@media screen and (max-width: 980px) {
  .more-designs__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .design__images img {
    max-width: 100%;
  }
}

@media screen and (max-width: 768px) {
  .more-designs__container {
    padding-left: 32px;
    padding-right: 32px;
  }
}

@media screen and (max-width: 540px) {
  .more-designs__header {
    font-size: 26px;
    font-weight: 300;
    line-height: 50px;
  }

  .more-designs__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }
}
</style>

<template>
  <div>
    <section class="invoicing__container">
      <p class="invoicing__header">Invoicing</p>
      <p class="invoicing__text">
        You can create and send invoices to your customers, and they can pay
        directly via a bank transfer or via the Kuda payment gateway. You can
        also create estimates (invoices that cannot be paid) and send to your
        customers to give an estimate of your service and said estimate can be
        converted to an invoice.
      </p>
    </section>

    <section class="invoicing__gallery__container">
      <section class="invoicing__gallery">
        <img :src="mainPicture" />
      </section>

      <section class="invoicing__gallery__menu">
        <div v-for="(picture, index) in pictures" v-bind:key="picture">
          <img
            :src="picture"
            @click="changemainPicture(index)"
            :class="{ active: index == indexofActive ? true : false }"
          />
        </div>
      </section>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      indexofActive: 0,
      mainPicture: require("../assets/images/invoicing-1.png"),
      pictures: [
        require("../assets/images/invoicing-1.png"),
        require("../assets/images/invoicing-2.png"),
        require("../assets/images/invoicing-3.png"),
      ],
    };
  },

  methods: {
    changemainPicture(index) {
      this.mainPicture = this.pictures[index];
      this.indexofActive = index;
    },
  },
};
</script>

<style scoped>
.invoicing__container {
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

.invoicing__header {
  font-family: "Graphik-Medium";
  font-size: 1.3rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.invoicing__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 1rem;
}

.invoicing__gallery__container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  /* max-width: 109.2rem; */
  margin: 0 128px;
  padding-top: 7rem;
  padding-bottom: 7rem;
  padding-left: 128px;
  padding-right: 128px;
  background-color: #000;
}

.invoicing__gallery {
  width: 544px;
  height: 518.63px;
  margin: 0 auto;
}

.invoicing__gallery img {
  width: 100%;
}

.invoicing__image__caption {
  margin: 70px 0;
  text-align: center;
  color: #fff;
  font-family: "Graphik-Regular";
  font-size: 1.1rem;
  font-weight: 300;
}

.invoicing__gallery__menu {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  margin-top: 150px;
  padding: 0 70px;
}

.invoicing__gallery__menu img {
  width: 99px;
  height: 63px;
  cursor: pointer;
}


.active {
  border: 3px solid #48d38a;
}

@media screen and (max-width: 980px) {
  .invoicing__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .invoicing__gallery__container {
    margin: 0 64px;
    padding-left: 64px;
    padding-right: 64px;
  }
}

@media screen and (max-width: 768px) {
  .invoicing__container {
    padding-left: 32px;
    padding-right: 32px;
  }

  .invoicing__gallery__container {
    margin: 0 32px;
    padding-left: 32px;
    padding-right: 32px;
  }
}
</style>

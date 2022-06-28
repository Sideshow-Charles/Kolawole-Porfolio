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

      <p class="invoicing__image__caption">
        {{ mainCaption }}
      </p>

      <section class="invoicing__gallery__menu">
        <div v-for="(pictures, index) in pictures" v-bind:key="index">
          <img
            :src="pictures.image"
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
      mainPicture: "",
      mainCaption: "",
      pictures: [
        {
          image: require("../assets/images/invoicing-1.png"),
          caption: "List of all the times user added on their invoice",
        },

        {
          image: require("../assets/images/invoicing-2.png"),
          caption: "Summary of the Invoice before it is sent to customer.",
        },

        {
          image: require("../assets/images/invoicing-3.png"),
          caption:
            "The various ways the invoice can be paid after the customer receives it",
        },
      ],
    };
  },

  methods: {
    changemainPicture(index) {
      this.mainPicture = this.pictures[index].image;
      this.mainCaption = this.pictures[index].caption;
      this.indexofActive = index;
    },
  },

  mounted() {
    (this.mainPicture = this.pictures[0].image),
      (this.mainCaption = this.pictures[0].caption);
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
  padding-left: 121px;
  padding-right: 121px;
}

.invoicing__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
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
  padding-left: 121px;
  padding-right: 121px;
  background-color: #000;
}

.invoicing__gallery {
  width: 75%;
  margin: 0 auto;
}

.invoicing__gallery img {
  width: 100%;
}

.invoicing__image__caption {
  margin-top: 70px;
  text-align: center;
  color: #fff;
  font-family: "Graphik-Regular";
  font-size: 1.1rem;
  font-weight: 300;
  line-height: 43px;
}

.invoicing__gallery__menu {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  margin-top: 70px;
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

  .invoicing__gallery__menu {
    margin-top: 70px;
    padding: 0 70px;
    gap: 25px;
    flex-wrap: wrap;
  }

  .invoicing__gallery img {
    width: 100%;
    margin-bottom: 70px;
  }
}

@media screen and (max-width: 540px) {
  .invoicing__header {
    font-size: 26px;
    font-weight: 300;
  }

  .invoicing__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 43px;
  }
}

</style>

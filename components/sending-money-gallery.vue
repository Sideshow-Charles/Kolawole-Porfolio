<template>
  <div>
    <section class="sending-money__container">
      <p class="sending-money__header">Sending Money</p>
      <div class="sending-money__text">
        Once you’ve signe up/in and you have access to your account, you can
        fund the account with your account number given to you and you can also
        send money to other banks with the following steps :
      </div>
      <ul class="sending-money__list">
        <li style="padding-left: 1em">
          Click on the Payments tab and go to “Send Money”
        </li>

        <li style="padding-left: 1em">
          Select Transaction type i.e Single Transaction
        </li>

        <li style="padding-left: 1em">
          Fill in the details of the person you are sending money to i.e Bank,
          Account Number and Amount
        </li>

        <li style="padding-left: 1em">Send Money</li>
      </ul>
    </section>

    <section class="sending-money__gallery__container">
      <section class="sending-money__gallery">
        <img :src="mainPicture" />
      </section>

      <p class="sending-money__image__caption">
        {{ mainCaption }}
      </p>

      <section class="sending-money__gallery__menu">
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
          image: require("../assets/images/sending-money1.png"),
          caption: "User selects the payment tab and clicks on Send Money",
        },
        {
          image: require("../assets/images/sending-money2.png"),
          caption: "User selects the bank they want to make payment to",
        },

        {
          image: require("../assets/images/sending-money3.png"),
          caption:
            "User fills in all the details and proceeds to sending money",
        },

        {
          image: require("../assets/images/sending-money4.png"),
          caption: "A confirmation page with the recipients name.",
        },

        {
          image: require("../assets/images/sending-money5.png"),
          caption: "User inputs their Transaction PIN",
        },

        {
          image: require("../assets/images/sending-money6.png"),
          caption: "Success message that the money has been sent",
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
.sending-money__container {
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

.sending-money__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.sending-money__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 2rem;
}

.sending-money__list {
  list-style-image: url("~assets/images/Polygon.png");
}

.sending-money__list li {
  margin-left: 20px;
  padding: 20px 0;
  font-family: "Graphik-Regular";
  font-size: 19px;
  font-weight: 400;
  line-height: 40px;
  letter-spacing: 0em;
  text-align: left;
}

.sending-money__gallery__container {
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

.sending-money__gallery {
  width: 75%;
  margin: 0 auto;
}

.sending-money__gallery img {
  width: 100%;
}

.sending-money__image__caption {
  margin-top: 70px;
  text-align: center;
  color: #fff;
  font-family: "Graphik-Regular";
  font-size: 1.1rem;
  font-weight: 300;
  line-height: 43px;
}

.sending-money__gallery__menu {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 61px;
  margin-top: 70px;
}

.sending-money__gallery__menu img {
  width: 99px;
  height: 63px;
  cursor: pointer;
}

.active {
  border: 3px solid #48d38a;
}

@media screen and (max-width: 1200px) {
  .sending-money__gallery__menu {
    flex-wrap: wrap;
  }
}

@media screen and (max-width: 980px) {
  .sending-money__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .sending-money__gallery__container {
    margin: 0 64px;
    padding-left: 64px;
    padding-right: 64px;
  }
}

@media screen and (max-width: 768px) {
  .sending-money__container {
    padding-left: 32px;
    padding-right: 32px;
  }

  .sending-money__gallery__container {
    margin: 0 24px;
    padding-left: 32px;
    padding-right: 32px;
  }

  .sending-money__gallery img {
    width: 100%;
  }

  .sending-money__gallery__menu {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    align-items: center;
    margin-top: 70px;
  }
}

@media screen and (max-width: 540px) {
  .sending-money__header {
    font-size: 26px;
    font-weight: 300;
  }

  .sending-money__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 43px;
  }

  .sending-money__list li {
    font-size: 18px;
    font-weight: 300;
    line-height: 43px;
  }
}
</style>

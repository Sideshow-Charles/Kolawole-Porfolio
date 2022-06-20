<template>
  <div>
      <section class="sending-money__container">
        <p class="sending-money__header">Sending Money</p>
         <div class="sending-money__text">Once you’ve signe up/in and you have access to your account, you can fund the account with your account number given to you and you can also send money to other banks with the following steps :</div>
           <ul class="sending-money__list">
            <li style="padding-left:1em">
              Click on the Payments tab and go to “Send Money”
            </li>

            <li style="padding-left:1em">
              Select Transaction type i.e Single Transaction
            </li>

            <li style="padding-left:1em">
              Fill in the details of the person you are sending money to i.e Bank, Account Number and Amount
            </li>

             <li style="padding-left:1em">
              Send Money
            </li>
          </ul>
    </section>

      <section class="sending-money__gallery__container">
          <section class="sending-money__gallery">
              <img :src = "mainPicture">
          </section>
      
    <section class="sending-money__gallery__menu">
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
      mainPicture: require("../assets/images/sending-money1.png"),
      pictures: [
        require("../assets/images/sending-money1.png"),
        require("../assets/images/sending-money2.png"),
        require("../assets/images/sending-money3.png"),
        require("../assets/images/sending-money4.png"),
        require("../assets/images/sending-money5.png"),
        require("../assets/images/sending-money6.png"),
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
.sending-money__container {
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
  padding-left: 128px;
  padding-right: 128px;
  background-color: #000;

}

.sending-money__gallery {
  width: 544px;
  height: 518.63px;
  margin: 0 auto;
}

.sending-money__gallery img {
  width: 100%;
}

.sending-money__image__caption {
  margin: 70px 0;
  text-align: center;
  color: #fff;
  font-family: "Graphik-Regular";
  font-size: 1.1rem;
  font-weight: 300;
}

.sending-money__gallery__menu {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 150px;
}

.sending-money__gallery__menu img {
  width: 99px;
  height: 63px;
  cursor: pointer;
}

.active {
  border: 3px solid #48D38A;
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
    margin: 0 32px;
    padding-left: 32px;
    padding-right: 32px;
  }
}
</style>

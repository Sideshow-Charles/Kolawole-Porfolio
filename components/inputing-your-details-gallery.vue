<template>
  <div>
    <section class="input-details__container">
      <p class="input-details__header">Inputing your Details</p>
      <div class="input-details__text">
        Once you select to sign up with Email, you are then asked to provide
        your email alongside other information that will be needed for you to
        set up your account. The necessary information that will be collected
        include ;
      </div>
      <ul class="input-details__list">
        <li style="padding-left: 1em">Verifying your ID with a selfie</li>

        <li style="padding-left: 1em">Uploading a valid ID card</li>

        <li style="padding-left: 1em">
          Filling a form that tells us more about your business
        </li>
      </ul>
    </section>

    <section class="input-details__gallery__container">
      <section class="input-details__gallery">
        <img :src="mainPicture" />
      </section>

      <p class="input-details__image__caption">
        {{ mainCaption }}
      </p>

      <section class="input-details__gallery__menu">
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
          image: require("../assets/images/input-details-1.png"),
          caption:
            "User signs up here with their basic details (Email Address) and password.",
        },
        {
          image: require("../assets/images/input-details-2.png"),
          caption:
            "User verifies their identity and tells us more about the business.",
        },

        {
          image: require("../assets/images/input-details-3.png"),
          caption:
            "User verifies their identity and tells us more about the business (Done state)",
        },

        {
          image: require("../assets/images/input-details-4.png"),
          caption: "Welcome screen once the user is done signing up.",
        },

        {
          image: require("../assets/images/input-details-5.png"),
          caption:
            "User selects what type of business account they want and they can see the features both types have",
        },

        {
          image: require("../assets/images/input-details-6.png"),
          caption: "User dashboard (Empty State)",
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
.input-details__container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  max-width: 109.2rem;
  margin: 0 auto;
  padding-top: 5rem;
  padding-bottom: 7rem;
  padding-left: 128px;
  padding-right: 128px;
}

.input-details__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.input-details__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 3rem;
}

.input-details__list {
  list-style-image: url("~assets/images/Polygon.png");
}

.input-details__list li {
  margin-left: 20px;
  padding: 20px 0;
  font-family: "Graphik-Regular";
  font-size: 19px;
  font-weight: 400;
  line-height: 40px;
  letter-spacing: 0em;
  text-align: left;
}

.input-details__gallery__container {
  margin: 0 128px;
  padding-top: 7rem;
  padding-bottom: 7rem;
  padding-left: 128px;
  padding-right: 128px;
  background-color: #000;
}

.input-details__gallery {
  width: 75%;
  margin: 0 auto;
}

.input-details__gallery img {
  width: 100%;
}

.input-details__image__caption {
  margin-top: 70px;
  text-align: center;
  color: #fff;
  font-family: "Graphik-Regular";
  font-size: 1.1rem;
  font-weight: 300;
  line-height: 43px;
}

.input-details__gallery__menu {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 61px;
  margin-top: 80px;
}

.input-details__gallery__menu img {
  width: 99px;
  height: 63px;
  cursor: pointer;
}

.active {
  border: 3px solid #48d38a;
}

@media screen and (max-width: 1200px) {
  .input-details__gallery__menu {
    flex-wrap: wrap;
  }
}

@media screen and (max-width: 980px) {
  .input-details__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .input-details__gallery__container {
    padding-left: 64px;
    padding-right: 64px;
    margin: 0 64px;
  }
}

@media screen and (max-width: 768px) {
  .input-details__container {
    padding-left: 32px;
    padding-right: 32px;
  }

  .input-details__gallery__container {
    padding-left: 32px;
    padding-right: 32px;
    margin: 0 32px;
  }

  .input-details__gallery__menu {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    align-items: center;
    margin-top: 50px;
  }
}

@media screen and (max-width: 540px) {
  .input-details__header {
    font-size: 26px;
    font-weight: 300;
  }

  .input-details__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 43px;
  }

  .input-details__list li {
    font-size: 18px;
    font-weight: 300;
    line-height: 43px;
  }
}
</style>

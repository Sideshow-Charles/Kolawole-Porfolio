<template>
  <div>
    <section class="visual-design__container">
      <p class="visual-design__header">Visual Design</p>
      <div class="visual-design__text">
        For the visual design the team worked with the
        <span>Agile methodology</span> and worked in sprints of 1 week, with
        each sprint we were able to design in order of importance starting from
        users being able to onboard to users being able to invite fellow users
        to join their courses till we got to the end. We opted for this
        methodology cause it was faster and helped us achieve more as a team
      </div>
    </section>

    <section class="visual-design__gallery__container">
      <section class="visual-design__gallery">
        <img :src="mainPicture" />
      </section>

      <p class="visual-design__image__caption">
        {{ mainCaption }}
      </p>

      <section class="visual-design__gallery__menu">
        <div v-for="(pictures, index) in pictures" v-bind:key="index">
          <img
            :src="pictures.image"
            @click="changemainPicture(index)"
            :class="{ active: index == indexofActive ? true : false }"
          />
        </div>
      </section>
    </section>

    <!-- Mobile gallery -->
    <section class="mobile__gallery">
      <div class="mobile-main__image">
        <img :src="mainPicture" />
      </div>
      <div class="navigation__buttons">
        <img
          src="../assets/images/citrone-left.svg"
          alt=""
          class="previous"
          @click="prev"
        />
        <img
          src="../assets/images/citrone-right.svg"
          alt=""
          class="next"
          @click="next"
        />
      </div>
      <p class="mobile__gallery__caption">
        {{ mainCaption }}
      </p>
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
          image: require("../assets/images/visual-design-1.png"),
          caption:
            "User signs up here with their basic details (Email Address) and password or they can sign up with their gmail or linkedin accounts.",
        },
        {
          image: require("../assets/images/visual-design-2.png"),
          caption: "User inputs their other details here",
        },

        {
          image: require("../assets/images/visual-design-3.png"),
          caption:
            "Upon sign up, you get to this screen to see what lessons or courses you are taking at the moment. (Empty State)",
        },

        {
          image: require("../assets/images/visual-design-4.png"),
          caption:
            "Upon sign up, you get to this screen to see what lessons or courses you are taking at the moment. ",
        },

        {
          image: require("../assets/images/visual-design-5.png"),
          caption:
            "This is the Admin portal, where the admin sees all the various academies that they are in control of.",
        },

        {
          image: require("../assets/images/visual-design-6.png"),
          caption:
            "Student Timeline for a particular course, here they can see different posts and communicate with tutors and fellow course members. ",
        },

        {
          image: require("../assets/images/visual-design-7.png"),
          caption: "Students answering quiz questions.",
        },

        {
          image: require("../assets/images/visual-design-8.png"),
          caption:
            "Students can view all their assignments for a particular course, their grades and the ones that haven’t been graded yet",
        },

        {
          image: require("../assets/images/visual-design-9.png"),
          caption:
            "Admin can see an overview of all the students on the platform and see how good or bad they are doing.",
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

    next() {
      if (this.indexofActive < this.pictures.length - 1) {
        this.indexofActive++;
        this.mainPicture = this.pictures[this.indexofActive].image;
        this.mainCaption = this.pictures[this.indexofActive].caption;
      } else {
        this.indexofActive = 0;
        this.mainPicture = this.pictures[0].image;
        this.mainCaption = this.pictures[0].caption;
      }
    },
    prev() {
      if (this.indexofActive > 0) {
        this.indexofActive--;
        this.mainPicture = this.pictures[this.indexofActive].image;
        this.mainCaption = this.pictures[this.indexofActive].caption;
      }
    },
  },

  mounted() {
    (this.mainPicture = this.pictures[0].image),
      (this.mainCaption = this.pictures[0].caption);
  },
};
</script>

<style scoped>
.visual-design__container {
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

.visual-design__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.visual-design__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 2rem;
}

.visual-design__gallery__container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  /* max-width: 109.2rem; */
  margin: 0 128px;
  padding-top: 7rem;
  padding-bottom: 7rem;
  padding-left: 16px;
  padding-right: 16px;
  background-color: #ffeaeb;
}

.visual-design__gallery {
  width: 75%;
  margin: 0 auto;
}

.visual-design__gallery img {
  width: 100%;
}

.visual-design__image__caption {
  margin-top: 70px;
  margin-left: auto;
  margin-right: auto;
  text-align: center;
  width: 50%;
  color: #000;
  font-family: "Graphik-Regular";
  font-size: 1.1rem;
  font-weight: 300;
  line-height: 43px;
}

.visual-design__gallery__menu {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 15px;
  margin-top: 70px;
}

.visual-design__gallery__menu img {
  width: 99px;
  height: 63px;
  cursor: pointer;
}

.active {
  border: 3px solid #f64f59;
}

.mobile__gallery {
  display: none;
}

@media screen and (max-width: 1200px) {
  .visual-design__gallery__menu {
    flex-wrap: wrap;
  }
}

@media screen and (max-width: 980px) {
  .visual-design__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .visual-design__gallery__container {
    margin: 0 64px;
    padding-left: 64px;
    padding-right: 64px;
  }
}

@media screen and (max-width: 768px) {
  .visual-design__container {
    padding-left: 32px;
    padding-right: 32px;
  }

  .visual-design__gallery__container {
    margin: 0 24px;
    padding-left: 32px;
    padding-right: 32px;
  }

  .visual-design__gallery img {
    width: 100%;
  }

  .visual-design__gallery__menu {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    align-items: center;
    margin-top: 70px;
  }
}

@media screen and (max-width: 540px) {
  .visual-design__header {
    font-size: 26px;
    font-weight: 300;
  }

  .visual-design__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 43px;
  }

  .visual-design__list li {
    font-size: 18px;
    font-weight: 300;
    line-height: 43px;
  }

  .visual-design__image__caption {
    width: 100%;
  }

  .visual-design__gallery__container {
    display: none;
  }

  .mobile__gallery {
    display: block;
    position: relative;
  }

  .mobile-main__image {
    background-color: #ffeaeb;
    margin: 0 32px;
  }

  .mobile-main__image img {
    padding-left: 32px;
    padding-right: 32px;
    max-width: 100%;
    padding-top: 32px;
    padding-bottom: 150px;
  }

  .navigation__buttons {
    margin: 0 32px;
    display: flex;
    justify-content: space-between;
    position: relative;
  }

  .previous {
    position: absolute;
    left: -1%;
    top: -300px;
    background: transparent;
    color: white;
  }

  .next {
    position: absolute;
    right: -1%;
    top: -300px;
    background: transparent;
    color: white;
  }

  .mobile__gallery__caption {
    font-size: 16px;
    font-weight: 300;
    line-height: 30px;
    font-family: "Graphik-Regular";
    position: absolute;
    text-align: center;
    top: 330px;
    color: #000;
    padding: 0 64px;
  }
}

@media screen and (max-width: 414px) {
  .navigation__buttons {
    margin: 0 32px;
    display: flex;
    justify-content: space-between;
    position: relative;
  }

  .previous {
    position: absolute;
    left: -1%;
    top: -255px;
    background: transparent;
  }

  .next {
    position: absolute;
    right: -1%;
    top: -255px;
    background: transparent;
  }

  .mobile__gallery__caption {
    font-size: 16px;
    font-weight: 300;
    line-height: 24px;
    font-family: "Graphik-Regular";
    position: absolute;
    text-align: center;
    top: 235px;
    padding: 0 64px;
  }
}

@media screen and (max-width: 320px) {
  .visual-design__header {
    font-size: 20px;
    font-weight: 300;
    line-height: 40px;
  }

  .visual-design__text {
    font-size: 15px;
    font-weight: 300;
    line-height: 40px;
  }

  .visual-design__list li {
    font-size: 15px;
    font-weight: 300;
    line-height: 40px;
  }

  .visual-design__gallery__container {
    padding-left: 16px;
    padding-right: 16px;
    margin: 0 16px;
  }

  .visual-design__image__caption {
    width: 100%;
    font-size: 15px;
    font-weight: 300;
    line-height: 40px;
  }

  .previous {
    top: -230px;
  }

  .next {
    top: -230px;
  }

  .mobile__gallery__caption {
    top: 180px;
    font-size: 13px;
  }
}

@media screen and (max-width: 280px) {
  .visual-design__container {
    padding-left: 16px;
    padding-right: 16px;
  }

   .previous {
    top: -220px;
  }

  .next {
    top: -220px;
  }

  .mobile__gallery__caption {
    top: 150px;
    font-size: 13px;
    padding: 0 48px;
  }
}
</style>

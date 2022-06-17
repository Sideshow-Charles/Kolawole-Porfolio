<template>
  <div>
    <Header></Header>
    <article class="product__container">
      <article class="product__header">
        <p>Citrone</p>
      </article>

      <article class="product__text">
        <p>
          Citrone is a learning platform that makes it easy for educators to
          <br />
          create learning experiences that engage students positively.
        </p>
      </article>

      <article class="role-description__container">
        <p>2021 - Present</p>
        <p>Type - Edutech</p>
        <p>Role - Product Designer</p>
        <p>Platform - Web Application</p>
      </article>
    </article>

    <section class="citrone-hero__image">
      <img src="../assets/images/citrone-hero-image.png" alt="" width="100%" />
    </section>

    <section class="about-product__container">
      <section class="product__brief">
        <p class="product__brief__header">Brief</p>
        <p class="product__brief__text">
          Education is a very integral part of our society today and the more we
          evolve the more education and learning evolves, thanks to the pandemic
          we had a lot of people pivoting to online classes and we realized some
          learning institutions do not use learning platforms therefore it is
          impossible to track student progress, amongst other numerous things
          and they just prefer to go the zoom (video calls) and email routes,
          this is where Citrone comes in, to provide a product that cares about
          the students and tutors.
        </p>
      </section>

        <section class="product__challenge">
        <p class="product__challenge__header">The challenge</p>
        <div class="product__challenge__text">
          <div class="product__challenge__list">
              <p>
              <span><img src="../assets/images/Polygon.png" alt="" /></span>How do we build a user friendly product that isn’t a big incovenience from sending notes and assignments by email.</p>

            <p>
              <span><img src="../assets/images/Polygon.png" alt="" /></span>How do we track student progress on assignments, lessons, tests etc.</p>

            <p>
              <span><img src="../assets/images/Polygon.png" alt="" /></span>How do we build a product where interaction between students and tutors, students and students is very seamless.</p>

            <p>
              <span><img src="../assets/images/Polygon.png" alt="" /></span>How do we ensure transparecy on the platform i.e students are able to see the scores for their quizzes and assignments and view a breakdown of how it was graded.</p>
          </div>
        </div>
    </section>
    <section class="product__role">
        <p class="product__role__header">My Role & the team</p>
        <p class="product__role__text">I was in charge of the design direction for this product, this involved color scheme selection, logo design, UI/UX research and design. I worked hand in hand with two engineers and a product manager to ship a user centered, usable and seamless learning platform.</p>
    </section>

    <section class="product-research__and__user__experience">
        <p class="product-research__and__user__experience__header">Research & User Experience</p>
        <p class="product-research__and__user__experience__text">For this product a lot of the research we did was user interview based, why? Because like I stated earlier we were trying to build something seamless, we wanted to convince people who were used to sending mails and having long zoom calls that there were better ways so we went to learning institutions and asked tutors and students what their current pain points were and we were able to gather useful data. Here is the feedback from some of the people we spoke to :</p>
    </section>

    <!-- <section class="research-points__container">
        <section class="research-individual__points">
            <img src="../assets/images/Johnson.png" alt="" width="80px" height="80px">
            <div class="research-individual__info">
            <p class="research-individual__name">Johnson</p>
            <p class="research-individual__role">Tutor, 35 years old</p>
            </div>
        </section> -->
        <!-- <p class="research-point__header">
                These are Mr Johnson’s current pain points on his <br> institutions current learning situation :
        </p>

         <ul class="input-details__lists">
              
              <span class="icon"><img src="../assets/images/Polygon.png" alt=""></span><li class="input-details__list">Has a hard time tracking his students progress</li>
         </ul>

           <ul class="input-details__lists">
              
              <span class="icon"><img src="../assets/images/Polygon.png" alt=""></span><li class="input-details__list">Wishes he could refer to old lesson notes in real time</li>
         </ul>

          <ul class="input-details__lists">
              
              <span class="icon"><img src="../assets/images/Polygon.png" alt=""></span><li class="input-details__list">His email is always a mess trying to sort out the <br> numerous assignments his tutors send to him to <br> grade.</li>
         </ul>

          <ul class="input-details__lists">
              
              <span class="icon"><img src="../assets/images/Polygon.png" alt=""></span><li class="input-details__list">There is a lot of room for cheating/plagiarism especially in quizzes.</li>
         </ul> 
    </section>-->
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

.citrone-hero__image {
  padding: 0 128px;
  max-width: 109.2rem;
  margin: 0 auto;
}

.citrone-hero__image img {
  width: 100%;
}

.about-product__container {
  display: flex;
  flex-direction: column;
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

.product-research__and__user__experience {
  margin-top: 3rem;
  margin-bottom: 2rem;
}

.product-research__and__user__experience__header {
  font-family: "Graphik-Medium";
  font-size: 1.7rem;
  font-weight: 900;
  margin-bottom: 2rem;
}

.product-research__and__user__experience__text {
  font-family: "Graphik-Regular";
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 3rem;
}

.research-points__container {
    padding: 0 48px;
}

.research-individual__points {
  display: flex;
  justify-content: space-between;
  align-items: center;
  /* padding: 0 48px; */
}

.research-individual__info {
    width: 62rem;
}

.research-individual__name {
  font-family: "Graphik-Medium";
  font-size: 1.1rem;
  font-weight: 900;
  /* margin-bottom: 1rem; */
}

.research-individual__role {
  font-family: "Graphik-Regular";
  font-size: 1rem;
  font-weight: 300;
  line-height: 3rem;
  /* margin-bottom: 3rem; */
}

.research-point__header {
  font-family: "Graphik-Regular";
  font-size: 1rem;
  font-weight: 300;
  line-height: 3rem;
  margin-top: 0.5rem;
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

  .citrone-hero__image {
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

  .citrone-hero__image {
    padding: 0 32px;
  }
}
</style>

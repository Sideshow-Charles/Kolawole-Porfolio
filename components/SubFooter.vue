<template>
  <div class="sub-footer">
    <section class="sub-footer__container">
      <section class="sub-footer__text">
        <p>
          Want to build something ground breaking and you feel I might <br />
          be the right fit? What are you waiting for
        </p>
      </section>
    </section>
    <footer class="footer__container">
      <footer class="footer__text">
        <p><span>&#169;</span>2022 Kolawole Popoola</p>
      </footer>
      <footer class="footer__links">
        <img src="../assets/images/twitter.svg" alt="" />
        <img src="../assets/images/linkedin.svg" alt="" />
        <img src="../assets/images/dribbble.svg" alt="" />
      </footer>
    </footer>
  </div>
</template>

<script>
</script>

<style scoped>
*{
    margin: 0;
    padding: 0;
}
.sub-footer {
  background: #f0f8fb;
}
.sub-footer__container {
  text-align: center;
  padding: 10rem 144px;
}

.sub-footer__text {
  margin-bottom: 1rem;
  line-height: 1.8;
  font-size: 1.5rem;
  font-weight: 500;
  font-family: "Graphik-Medium";
}

.footer__container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 128px;
  max-width: 109.2rem;
  margin: 0 auto;
  padding-bottom: 32px;
}

.footer__text {
  font-size: 1.2rem;
  font-family: "Graphik-Regular";
  font-weight: 300;
}

.footer__links {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 15%;
}

@media screen and (max-width: 968px) {
  .footer__container {
    padding-left: 64px;
    padding-right: 64px;
  }
}

@media screen and (max-width: 768px) {
  .sub-footer__container {
    padding: 7rem 64px;
  }

  .sub-footer__text {
    font-size: 1.3rem;
  }

  .footer__container {
    padding-left: 24px;
    padding-right: 24px;
  }

  .footer__links {
    width: 20%;
  }

  .footer__text {
    font-size: 0.8em;
  }

  .footer__links img {
    width: 15%;
  }
}
</style>

<template>
  <footer class="footer__container">
    <footer class="footer__text">
      <p><span>&#169;</span>2022 Kolawole Popoola</p>
    </footer>
    <footer class="footer__links">
      <img src="../assets/images/twitter.png" alt="" />
      <img src="../assets/images/linkedin.png" alt="" />
      <img src="../assets/images/dribble.png" alt="" />
    </footer>
  </footer>
</template>

<script>
import fonts from "../assets/fonts/fonts.css";
export default {
  fonts,
};
</script>

<style scoped>
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

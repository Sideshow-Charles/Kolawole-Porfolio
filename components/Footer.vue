<template>
  <footer class="footer__container">
    <footer class="footer__text">
      <p>&copy; {{ new
        Date().getFullYear() }} Kolawole Popoola</p>
    </footer>
    <footer class="footer__links">
      <a href="https://www.twitter.com/_Kolaa" target="_blank"><img src="../assets/images/twitter.svg" alt="" /></a>
      <a href="https://www.linkedin.com/in/kolawole-popoola-b61664143" target="_blank"><img
          src="../assets/images/linkedin.svg" alt="" /></a>
      <a href="https://www.dribbble.com/_Kolaa" target="_blank"><img src="../assets/images/dribbble.svg" alt="" /></a>
    </footer>
  </footer>
</template>

<script></script>

<style scoped>
.footer__container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 121px;
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

@media screen and (max-width: 980px) {
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

@media screen and (max-width: 540px) {
  .footer__text {
    font-size: 1em;
  }

  .footer__links img {
    width: 100%;
  }
}

@media screen and (max-width: 320px) {
  .footer__text {
    font-size: 0.7em;
  }
}
</style>

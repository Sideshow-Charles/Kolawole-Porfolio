<template>
  <div class="nav__bar">
    <div class="nav__items__left">
      <div class="logo__container">
        <Nuxt-Link to="/"><img src="../assets/images/KOLAWOLE.svg" alt="" /></Nuxt-Link>
      </div>
      <ul class="nav__items__center">
        <li class="nav__item__center"><NuxtLink to="/work">Work</NuxtLink></li>
        <li class="nav__item__center"><NuxtLink to="/about">About</NuxtLink></li>
        <li class="nav__item__center"><NuxtLink to="/design">Design</NuxtLink></li>
        <li class="nav__item__center"><NuxtLink to="/resume">Resume</NuxtLink></li>
      </ul>
    </div>
    <div class="nav__items__right">
      <Button></Button>
    </div>
  </div>
</template>

<script>
import fonts from "../assets/fonts/fonts.css"
export default {
components: {
    fonts
}
}
</script>

<style scoped>
.nav__bar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 109.2rem;
  margin: 0 auto;
  padding-left: 128px;
  padding-right: 128px;
  padding-top: 40px;
  padding-bottom: 20px;
}

.nav__items__left {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 60%;
}

.nav__items__left a {
  text-decoration: none;
  color: inherit;
}

.nav__items__left a:active {
  text-decoration: underline;
}

.nav__items__center {
  display: flex;
  justify-content: space-around;
  width: 65%;
  font-family: "Graphik";
  font-weight: 400;
  font-size: 18px;
}

.nav__item__center {
  display: flex;
  justify-content: space-between;
}

/* Media Queries */
@media screen and (max-width: 968px) {
  .nav__bar {
    padding-left: 64px;
    padding-right: 64px;
  }
}

@media screen and (max-width: 768px) {
  .nav__bar {
    padding-left: 24px;
    padding-right: 24px;
  }

  .nav__items__center {
    display: none;
  }

  .nav__items__right {
    display: none;
  }
}
</style>
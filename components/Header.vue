<template>
  <div class="nav__bar">
    <div class="nav__items__left">
      <div class="logo__container">
        <Nuxt-Link to="/"
          ><img src="../assets/images/KOLAWOLE.svg" alt=""
        /></Nuxt-Link>
      </div>
      <ul class="nav__items__center">
        <li class="nav__item__center">
          <Nuxt-Link to="/kuda-business-banking">Work</Nuxt-Link>
        </li>
        <li class="nav__item__center">
          <Nuxt-Link to="/about">About</Nuxt-Link>
        </li>
        <li class="nav__item__center">
          <Nuxt-Link to="/designs">Designs</Nuxt-Link>
        </li>
        <li class="nav__item__center">
          <a href="https://drive.google.com/file/d/1xaHKXFhbjV5YDqtI1Y25RXKpGkmJbA-L/view?usp=sharing">Resume</a>
        </li>
      </ul>
    </div>
    <div class="nav__items__right">
      <Button></Button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.nav__bar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 109.2rem;
  margin: 0 auto;
  padding-left: 120px;
  padding-right: 120px;
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

.nav__items__center {
  display: flex;
  justify-content: space-around;
  width: 65%;
  font-family: "Graphik-Regular";
  font-weight: 400;
  font-size: 18px;
}

.nav__items__center a:active,
.nav__items__center a.nuxt-link-active {
  border-bottom: 3px solid #14586d;
}

.nav__item__center {
  display: flex;
  justify-content: space-between;
}

/* Media Queries */
@media screen and (max-width: 1024px) {
  .nav__items__left {
    width: 65%;
  }

  .nav__items__center {
    font-size: 16px;
    width: 60%;
  }
}

@media screen and (max-width: 980px) {
  .nav__bar {
    padding-left: 64px;
    padding-right: 64px;
  }

  .nav__items__left {
    flex-direction: column;
    align-items: flex-start;
  }

  .nav__items__center {
    width: 100%;
    margin-top: 37px;
    justify-content: space-between;
  }

  .nav__items__right {
    display: none;
  }

  .nav__items__left {
    width: 100%;
  }
}

@media screen and (max-width: 820px) {
  .nav__items__center {
    width: 100%;
  }
}

@media screen and (max-width: 768px) {
  .nav__bar {
    padding-left: 32px;
    padding-right: 32px;
    flex-direction: column-reverse;
  }
}

@media screen and (max-width: 540px) {
  .nav__items__center {
    font-size: 17px;
    font-weight: 300;
    line-height: 43px;
  }
}

@media screen and (max-width: 320px) {
   .nav__items__left {
    /* width: 65%; */
    gap: 0;
  }

    .nav__items__center {
    font-size: 13px;
    font-weight: 300;
    line-height: 43px;
  }
}

@media screen and (max-width: 280px) {
  .nav__bar {
    padding-left: 16px;
    padding-right: 16px;
  }
}
</style>

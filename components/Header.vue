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
          <Nuxt-Link to="/resume">Resume</Nuxt-Link>
        </li>
      </ul>
    </div>
    <div class="nav__items__right">
      <Button></Button>
    </div>

    <!-- <img src="../assets/images/Menu.svg" alt="hamburger-menu" class="hamburger__menu" @click="toggleMobileNav" v-show="mobile"> -->

    <!-- Mobile nav -->
    <!-- <div class="mobile__nav" v-show="mobile">
      <ul class="mobile__nav__links">
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
          <Nuxt-Link to="/resume">Resume</Nuxt-Link>
        </li>
      </ul>
    </div> -->
    <!-- End of Mobile nav -->
  </div>
</template>

<script>
export default {
  // data() {
  //   return {
  //     mobileNav: null,
  //     mobile: null,
  //     windowWidth: null,
  //     dropDown: false,
  //   };
  // },
  // mounted() {
  //   window.addEventListener("resize", this.checkScreen);
  //   this.checkScreen();
  // },
  // methods: {
  //   toggleMobileNav() {
  //  this.mobileNav = !this.mobileNav
  // },
  //  showdropDown() {
  //    this.dropDown = !this.dropDown
  //  },
  //  hidedropDown() {
  //    if (this.dropDown = true) {
  //       this.dropDown = false;
  //    }
  //  },
  // Checks the screen size to show or hide the mobile nav.
  //   checkScreen() {
  //     this.windowWidth = window.innerWidth;
  //     if (this.windowWidth <= 980) {
  //       this.mobile = true;
  //       return;
  //     }
  //     this.mobile = false;
  //     this.mobileNav = false;
  //     return;
  //   },
  // },
};
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
    width: 50%;
    margin-top: 50px;
    justify-content: space-between;
  }

  .nav__items__right {
    display: none;
  }

  .nav__items__left {
    width: 100%;
  }
}

@media screen and (max-width: 768px) {
  .nav__bar {
    padding-left: 32px;
    padding-right: 32px;
    flex-direction: column-reverse;
  }

  .nav__items__center {
    width: 100%;
  }
}

@media screen and (max-width: 540px) {
  .nav__items__center {
    font-size: 17px;
    font-weight: 300;
    line-height: 43px;
  }
}
</style>

<template>
  <div class="nav__bar">
    <div class="nav__items__left">
      <div class="logo__container">
        <Nuxt-Link to="/"><img src="../assets/images/KOLAWOLE.svg" alt="" /></Nuxt-Link>
      </div>
      <ul class="nav__items__center">
        <li class="nav__item__center"><Nuxt-Link to="/work">Work</Nuxt-Link></li>
        <li class="nav__item__center"><Nuxt-Link to="/about">About</Nuxt-Link></li>
        <li class="nav__item__center"><Nuxt-Link to="/design">Designs</Nuxt-Link></li>
        <li class="nav__item__center"><Nuxt-Link to="/resume">Resume</Nuxt-Link></li>
      </ul>
    </div>
    <div class="nav__items__right">
      <Button></Button>
    </div>


      <img src="../assets/images/Menu.svg" alt="hamburger-menu" class="hamburger__menu" @click="toggleMobileNav" v-show="mobile">

       <!-- Mobile nav -->
    <div class="mobile__nav" v-show="mobileNav">
      <ul class="mobile__nav__links">
        <Nuxt-Link to="#"><li class="mobile__nav__link">Work</li></Nuxt-Link>
        <Nuxt-Link to="#"><li class="mobile__nav__link">About</li></Nuxt-Link>
        <Nuxt-Link to="#"><li class="mobile__nav__link">Designs</li></Nuxt-Link>
        <Nuxt-Link to="#"><li class="mobile__nav__link">Resume</li></Nuxt-Link>
    
        <Button></Button>

      </ul>
    </div>
    <!-- End of Mobile nav -->
  </div>
</template>

<script>
export default {
       data () {
       return {
          mobileNav: null,
          mobile: null,
          windowWidth: null,
          dropDown: false,
       }
     },

    mounted () {
       window.addEventListener("resize", this.checkScreen);
       this.checkScreen();
    },

     methods: {
       toggleMobileNav() {
         this.mobileNav = !this.mobileNav
       },
       
       showdropDown() {
         this.dropDown = !this.dropDown
       },

       hidedropDown() {
         if (this.dropDown = true) {
            this.dropDown = false;
         }
       },

       // Checks the screen size to show or hide the mobile nav. 

       checkScreen() {
         this.windowWidth = window.innerWidth;
         if (this.windowWidth <= 980) {
           this.mobile = true;
           return;
         } 
        this.mobile = false;
        this.mobileNav = false;
        return;
       },
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
  border-bottom: 3px solid #14586D;
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

  .nav__items__center {
    display: none;
  }

  .nav__items__right {
    display: none;
  }

   .hamburger__menu {
    height: 35px;
    width: 25px;
    cursor: pointer;
    margin-bottom: 5px;

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


.mobile__nav {
  display: flex;
  flex-direction: column;
  align-items: center;
  background: #f0f8fb;
  width: 100%;
  position: fixed;
  left: 0;
  height: 100vh;
  /* overflow: none; */
  padding-top: 200px;
  overflow-x: hidden;
  /* z-index: 999; */
}

.mobile__nav__links li {
 padding-top: 25px;
  list-style: none;
  text-align: center;
  margin-top: 25px;
  position: relative;
  top: 0;
  overflow: hidden;
}


</style>
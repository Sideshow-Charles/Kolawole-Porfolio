<template>
  <a href="mailto:kolapopoola4@gmail.com"
    ><button
      class="contact"
      :class="btnStyle"
      v-bind="$attrs"
      v-on="$listeners"
    >
      <slot /> <span class="emoji">&#128075;&#127997;</span> Contact Me!
    </button></a
  >
</template>

<script>
export default {
  name: "Contact",
  props: {
    btnStyle: {
      type: String,
      default: "",
    },
  },
};
</script>

<style scoped>
.contact {
  background-color: #14586d;
  padding-top: 7px;
  padding-bottom: 7px;
  padding-left: 20px;
  padding-right: 20px;
  color: #fff;
  border: none;
  border-radius: 5px;
  font-family: "Graphik-Regular";
  font-weight: 400;
  font-size: 1.1em;
  cursor: pointer;
}

.contact:hover {
  background: #0a4557;
  transition: 0.5s all ease-in-out;
}

span.emoji {
  font-size: 18px;
  vertical-align: middle;
  line-height: 2;
  margin-right: 5px;
}

@media screen and (max-width: 540px) {
  .mobile {
    margin-top: 10px;
    width: 100%;
  }
}
</style>

<template>
  <button class="contact">
    <span class="emoji">&#128075;&#127997;</span> Contact Me!
  </button>
</template>

<script>
import fonts from "../assets/fonts/fonts.css";
export default {
  fonts,
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
  font-family: "Graphik";
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
</style>
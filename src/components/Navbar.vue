<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-primary px-3">
    <router-link class="navbar-brand d-flex" :to="{ name: 'Home' }">
      <div class="d-flex flex-column align-items-center">
        <!-- <img alt="logo" src="../assets/img/cw-logo.png" height="45" /> -->
        <h2>JAMES MUSCHLER</h2>
      </div>
    </router-link>
    <button
      class="navbar-toggler"
      type="button"
      data-bs-toggle="collapse"
      data-bs-target="#navbarText"
      aria-controls="navbarText"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon" />
    </button>
    <div class="collapse navbar-collapse" id="navbarText">
      <ul class="navbar-nav me-auto">
        <li>
          <div class="btn text-success lighten-30 selectable text-uppercase">
            BIO
          </div>
        </li>
        <li>
          <div class="btn text-success lighten-30 selectable text-uppercase">
            Lessons
          </div>
        </li>
      </ul>
      <Socials />
      <!-- LOGIN COMPONENT HERE -->
      <!-- <Login /> -->
    </div>
  </nav>
</template>

<script>
import Socials from "./Socials.vue";
// var Vue = require("vue");
// var VueScrollTo = require("vue-scrollto");

// Vue.use(VueScrollTo);

// You can also pass in the default options
// Vue.use(VueScrollTo, {
//   container: "body",
//   duration: 500,
//   easing: "ease",
//   offset: 0,
//   force: true,
//   cancelable: true,
//   onStart: false,
//   onDone: false,
//   onCancel: false,
//   x: false,
//   y: true,
//});
export default {
  // directives: {
  //   VueScrollTo,
  // },
  setup() {
    return {};
  },
  components: { Socials },
};
</script>

<style scoped>
a:hover {
  text-decoration: none;
}
.nav-link {
  text-transform: uppercase;
}
.navbar-nav .router-link-exact-active {
  border-bottom: 2px solid var(--bs-success);
  border-bottom-left-radius: 0;
  border-bottom-right-radius: 0;
}
</style>

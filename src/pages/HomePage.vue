<template>
  <header>
    <Navbar @scroll="scrollToElement" />
  </header>
  <div class="">
    <img
      class="img-fluid"
      src="src/assets/img/MFY1J0.jpg"
      alt="Image of James at the drumset"
    />
  </div>

  <div id="bio" class="bio container-fluid" ref="bio">
    <div class="row">
      <div class="col-md-6">
        <h1 class="text-primary text-center">BIO</h1>
        <h3 class="">James Muschler</h3>
        <p class="p-2 my-2 elevation-4 rounded">
          is an American multi-instrumentalist, composer, and producer from
          Cleveland, Ohio. He specializes in drums, tabla, piano, saxophone,
          guitar, bass, bansuri flute, and various frame drums. <br />
          He earned a BFA in Jazz Performance (drums) from The New School for
          Jazz and Contemporary Music in NYC. James co-founded Moon Hooch with
          Wenzl McGowen and Michael Wilbur in 2010. For ten years, they toured
          the US, Europe, Serbia, Russia, Australia, and Canada, playing major
          festivals and venues. <br />
          James teaches drums, tabla, piano, and saxophone in Park Slope,
          Brooklyn, remotely, or in-home within the NYC area. He has experience
          with adults and youth ages 5+. <br />
          <strong> Reach James at: </strong>
          <a href="mailto:jamesmuschler@gmail.com">jamesmuschler@gmail.com</a>
        </p>
      </div>
      <div class="col-md-6">
        <img
          class="img-fluid"
          src="src/assets/img/Jane and James - Masters-195.jpg"
          alt=""
        />
      </div>
    </div>
  </div>
  <Carousel2 />
</template>

<script>
import { ref } from "vue";
import Navbar from "../components/Navbar.vue";
import Carousel from "../components/Carousel.vue";
import Carousel2 from "../components/Carousel2.vue";

export default {
  name: "Home",
  methods: {
    scrollToElement(target) {
      let el = this.$refs[target];
      if (el) {
        el.scrollIntoView({ behavior: "smooth" });
      }
    },
  },
  setup() {
    return {
      bio: ref.bio,
    };
  },
  components: { Navbar, Carousel, Carousel2 },
};
</script>

<style scoped lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Raleway&display=swap");
#bio {
  font-family: "Raleway", sans-serif;
}
.home {
  display: grid;
  height: 80vh;
  place-content: center;
  text-align: center;
  user-select: none;
  .home-card {
    width: 50vw;
    > img {
      height: 200px;
      max-width: 200px;
      width: 100%;
      object-fit: contain;
      object-position: center;
    }
  }
}
</style>

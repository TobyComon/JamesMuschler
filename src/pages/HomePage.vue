<template>
  <header>
    <Navbar @scroll="scrollToElement" />
  </header>
  <div class="bg-black">
    <img
      class="w-75"
      src="src/assets/img/MFY1J0.jpg"
      alt="Image of James at the drumset"
    />
    <span class="position-absolute text-white text-center landing-text"
      ><h1>James Muschler</h1>
      <b class=""
        >Instrumentalist <i class="mdi px-2 mdi-triangle"></i> Composer
        <i class="px-2 mdi mdi-triangle"></i> Producer</b
      >
    </span>
  </div>

  <div id="bio" class="bio container-fluid bg-black" ref="bio">
    <div class="row">
      <div class="col-md-6 p-lg-5">
        <p class="fs-1 text-primary p-5">Who is James?</p>

        <p class="p-4 text-white my-2 elevation-4 rounded">
          James Muschler is an American multi-instrumentalist, composer, and
          producer from Cleveland, Ohio. He specializes in drums, tabla, piano,
          saxophone, guitar, bass, bansuri flute, and various frame drums.
          <br />
        </p>

        <p class="p-4 text-primary my-2 elevation-4 rounded">
          He earned a BFA in Jazz Performance (drums) from The New School for
          Jazz and Contemporary Music in NYC. James co-founded Moon Hooch with
          Wenzl McGowen and Michael Wilbur in 2010. For ten years, they toured
          the US, Europe, Serbia, Russia, Australia, and Canada, playing major
          festivals and venues. <br />
        </p>

        <p class="p-4 text-white my-2 elevation-4 rounded">
          James teaches drums, tabla, piano, and saxophone in Park Slope,
          Brooklyn, remotely, or in-home within the NYC area. He has experience
          with adults and youth ages 5+. <br />
        </p>
      </div>
      <div class="col-md-6 p-5">
        <img
          class="w-75 bio-image"
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

.landing-text {
  top: 50vh;
  @media (orientation: landscape) {
    right: 10vh;
  }
  @media (orientation: portrait) {
    padding: 1em;
    background: rgba(0, 0, 0, 0.495);
    top: 20vh;
    right: 1vh;
  }
}
</style>

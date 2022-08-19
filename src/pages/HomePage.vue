<template>
  <div class="">
    <img
      class="img-fluid"
      src="src/assets/img/MFY1J0.jpg"
      alt="Image of James at the drumset"
    />
  </div>

  <div id="bio" class="bio container-fluid">
    <div class="row">
      <div class="col-md-6">
        <h1 class="text-primary">BIO</h1>
        <article class="bg-dark text-light p-2 my-2 rounded shadow">
          I believe in the power of music to bring people together. I am an
          American multi-instrumentalist/composer/producer from Cleveland, OH.
          My instruments include the drums, tabla, piano, saxophone, guitar,
          bass, bansuri flute, and various frame drums. In 2011, I graduated
          from The New School for Jazz and Contemporary Music in NYC with a BFA
          in Jazz Performance (drums). In 2010, I co-founded the band Moon Hooch
          with saxophonists Wenzl McGowen and Michael Wilbur. We toured for 10
          years, playing at major festivals and venues in the US and in Europe,
          as well as Serbia, Russia, and Australia. I'm currently based in the
          New England area (Burlington, VT). In February 2021, I released my
          debut album, "The Evolution of Life Forms on Earth", a 40-minute
          musical simulation of our 4-billion year biological ancestry (written
          for acoustic percussion). I am teaching music remotely until the
          pandemic situation improves. Connect with me at
          jamesmuschler@gmail.com. I love teaching, and I love receiving
          feedback (: <br />
          I am also passionate about environmentalism and of the preservation of
          animal habitat and of biodiversity. One of the most direct ways we can
          all contribute positively to the future of the planet is to acquire a
          vegan diet. I run a vegan cooking blog on instagram
          <a href="">@cookinginthecave </a>
        </article>
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";

export default {
  name: "Home",

  setup() {
    return {
      bio: ref.bio,
    };
  },
};
</script>

<style scoped lang="scss">
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

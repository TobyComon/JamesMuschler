<template>
  <div
    id="carouselExampleIndicators"
    class="carousel slide"
    data-ride="carousel"
  >
    <ol class="carousel-indicators">
      <li
        data-target="#carouselExampleIndicators"
        data-slide-to="0"
        class="active"
      ></li>
      <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
      <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
    </ol>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img
          class="d-block w-100"
          src="src/assets/img/evolutionoflifeformsonearth.webp"
          alt="First slide: The Evolution Of Life Forms On Earth"
        />
        <div
          class="
            p-2
            bg-gradient bg-grey
            elevation-3
            card
            carousel-caption
            d-none d-md-block
          "
        >
          <h5 class=""><a href=""></a> The Evolution of Life Forms on Earth</h5>
          <h6>2021</h6>
          <p class="text-start">
            The Evolution of Life Forms on Earth is a 40-minute musical
            simulation of our 4-billion year biological ancestry, using sound
            (acoustic percussion) as a medium to express the fossil record (in
            terms of rates of genetic change, relative biodiversity, and mass
            extinction events). In the piece, sound = life, and sonic complexity
            and high volume equates to thriving ecosystems. Low volume and
            removal of most layers of sound equates to an extinction event, with
            a new lineage of sounds taking its place until the next extinction
            event, representing the eons, eras, and periods that shaped the
            evolution of life on Earth. In this way, the listener is able to
            experience a simulation of life's story in an abstract, yet
            understandable way. You can find The Evolution of Life Forms on
            Earth on Spotify under "James Muschler", on iTunes, Google Play,
            Amazon Music, etc. and also on my band camp page :
            jamesmuschler.bandcamp.com
          </p>
        </div>
      </div>
      <div class="carousel-item">
        <img
          class="d-block w-100"
          src="src/assets/img/moonhooch.webp"
          alt="Second slide: Moon Hooch - Moon Hooch"
        />
      </div>
      <div
        class="
          p-2
          bg-gradient bg-grey
          elevation-3
          card
          carousel-caption
          d-none d-md-block
        "
      ></div>
      <div class="carousel-item">
        <img class="d-block w-100" src="..." alt="Third slide" />
      </div>
    </div>
    <a
      class="carousel-control-prev"
      href="#carouselExampleIndicators"
      role="button"
      data-slide="prev"
    >
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="sr-only">Previous</span>
    </a>
    <a
      class="carousel-control-next"
      href="#carouselExampleIndicators"
      role="button"
      data-slide="next"
    >
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="sr-only">Next</span>
    </a>
  </div>
</template>


<script>
export default {
  setup() {
    return {};
  },
};
</script>


<style lang="scss" scoped>
</style>
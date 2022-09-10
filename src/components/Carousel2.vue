<template>
  <div class="component">
    <div id="carouselId" class="carousel slide" data-bs-ride="carousel">
      <ol class="carousel-indicators">
        <li
          data-bs-target="#carouselId"
          data-bs-slide-to="0"
          class="active"
          aria-current="true"
          aria-label="First slide"
        ></li>
        <li
          data-bs-target="#carouselId"
          data-bs-slide-to="1"
          aria-label="Second slide"
        ></li>
        <li
          data-bs-target="#carouselId"
          data-bs-slide-to="2"
          aria-label="Third slide"
        ></li>
      </ol>
      <div class="carousel-inner" role="listbox">
        <div class="carousel-item active">
          <img
            src="src/assets/img/evolutionoflifeformsonearth.webp"
            class="w-100 d-block"
            alt="First slide"
          />
          <div
            class="carousel-caption d-none d-md-block bg-black bg-opacity-50"
          >
            <h3>The Evolution of Life Forms on Earth</h3>
            <p>Description</p>
          </div>
        </div>
        <div class="carousel-item">
          <img
            src="src/assets/img/moonhooch.webp"
            class="w-100 d-block"
            alt="Second slide"
          />
          <div
            class="carousel-caption d-none d-md-block bg-black bg-opacity-50"
          >
            <h3>Title</h3>
            <p>Description</p>
          </div>
        </div>
        <div class="carousel-item">
          <img
            src="holder.js/900x500/auto/#666:#444/text:Third slide"
            class="w-100 d-block"
            alt="Third slide"
          />
          <div
            class="carousel-caption d-none d-md-block bg-black bg-opacity-50"
          >
            <h3>Title</h3>
            <p>Description</p>
          </div>
        </div>
      </div>
      <button
        class="carousel-control-prev"
        type="button"
        data-bs-target="#carouselId"
        data-bs-slide="prev"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button
        class="carousel-control-next"
        type="button"
        data-bs-target="#carouselId"
        data-bs-slide="next"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>
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
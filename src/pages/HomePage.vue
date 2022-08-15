<template>
  <div
    class="
      home
      flex-grow-1
      d-flex
      flex-column
      align-items-center
      justify-content-center
    "
  >
    <div class="home-card p-5 bg-white rounded elevation-3 mb-5">
      <img
        src="https://bcw.blob.core.windows.net/public/img/8600856373152463"
        alt="CodeWorks Logo"
        class="rounded-circle"
      />
      <h1 class="my-5 bg-dark text-white p-3 rounded text-center">
        Vue 3 Starter
      </h1>
    </div>
  </div>
  <div class="container my-5">
    <div class="row">
      <div class="col">
        <img src="https://thiscatdoesnotexist.com" alt="" />
      </div>
    </div>
  </div>
  <div id="bio" class="mt-5 bio container-fluid d-flex flex-grow-1">
    <div class="row">
      <div class="col">
        BIO Lorem ipsum dolor, sit amet consectetur adipisicing elit. Labore,
        recusandae! Nulla id cumque ut quibusdam recusandae architecto neque
        odio quisquam? Suscipit veniam voluptate alias esse vitae non modi amet
        qui? Lorem, ipsum dolor sit amet consectetur adipisicing elit. Molestiae
        temporibus sunt earum, ullam tenetur nemo atque eligendi perferendis,
        rem porro animi adipisci dolore quo hic laudantium sint cum magni sequi.
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sed dicta
        ullam impedit neque in cum explicabo, cumque sunt expedita laudantium
        tempore, amet ea unde, rem blanditiis dolor? Incidunt, animi quis?
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

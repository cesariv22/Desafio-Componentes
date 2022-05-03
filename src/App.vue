<template>
  <div id="app" class="ms-4 my-5">
    <div>
      <ImagenRick :imgperso="imagenes" />
    </div>
  </div>
</template>

<script>
import ImagenRick from "@/components/ImagenRick.vue";

export default {
  name: "App",
  data() {
    return {
      imagenes: [
        {
          nombre: "Rick Sanchez",
          src: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
        },
        {
          nombre: "Morty Smith",
          src: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
        },
        {
          nombre: "Summer Smith",
          src: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
        },
        {
          nombre: "Beth Smith",
          src: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
        },
        {
          nombre: "Jerry Smith",
          src: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
        },
      ],
    };
  },
  components: {
    ImagenRick,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
body {
  background-image: url(https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png);
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
}
</style>

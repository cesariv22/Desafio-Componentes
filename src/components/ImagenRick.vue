<template>
  <div class="mt-4">
    <div v-for="(imagen, i) in imgperso" :key="i">
      <img
        :src="imagen.src"
        :alt="imagen.nombre"
        class="img-rick"
        width="120"
      />
      <p class="d-inline ms-3 name-rick">{{ imagen.nombre }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "ImagenRick",
  props: {
    imgperso: {
      type: Array,
      default: () => [],
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.name-rick {
  font-size: 40px;
  font-family: cursive;
  color: deepskyblue;
}
.img-rick {
  border-radius: 50%;
  width: 120px;
  margin-top: 1rem;
}
</style>

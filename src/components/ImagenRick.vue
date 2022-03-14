<template>
  <div class="d-flex mt-4">
    <div>
      <img
        :src="imgperso.src"
        :alt="imgperso.nombre"
        class="img-rick"
        width="120"
      />
      <p class="d-inline ms-3 name-rick">{{ imgperso.nombre }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "ImagenRick",
  props: {
    imgperso: {
      type: Object,
      default: () => {},
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
}
</style>

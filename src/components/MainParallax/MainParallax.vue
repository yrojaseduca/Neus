<template>
  <v-parallax src="https://cdn.vuetifyjs.com/images/parallax/material.jpg">
  <div class="MainParallaxContent">
    <p>aqui una frase tuya y foto de fondo</p>
  </div>
  </v-parallax>
</template>

<script>
    export default {
        name: 'MainParallax'
    };
</script>

<style scoped>
  .MainParallaxContent{
    display: flex;
    justify-content: center;
    height: 100%;
    align-items: center;
  }
</style>

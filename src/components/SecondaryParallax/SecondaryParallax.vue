<template>

  <v-parallax src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg">
  <div class="SecondaryParallax">
    <p>aqui contenido noticias en un slider??</p>
  </div>
  </v-parallax>
</template>

<script>
    export default {
        name: 'SecondaryParallax'
    };
</script>

<style scoped>
  .SecondaryParallax{
    display: flex;
    justify-content: center;
    height: 100%;
    align-items: center;
  }
</style>

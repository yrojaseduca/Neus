<template>
  <NavBar />
  <MainParallax />
  <HelloWorld />
  <SecondaryParallax />
  <WhatsApp />
  <CustomFooter />
</template>

<script>
import { defineComponent } from 'vue';

// Components
import HelloWorld from '../components/HelloWorld.vue';
import CustomFooter from "@/components/CustomFooter/CustomFooter.vue";
import WhatsApp from "@/components/WhatsApp/WhatsApp.vue";
import MainParallax from "@/components/MainParallax/MainParallax.vue";
import SecondaryParallax from "@/components/SecondaryParallax/SecondaryParallax.vue";
import NavBar from "@/components/NavBar/NavBar.vue";
export default defineComponent({
  name: 'HomeView',

  components: {
    HelloWorld,
    CustomFooter,
    WhatsApp,
    MainParallax,
    SecondaryParallax,
    NavBar,
  },
});
</script>

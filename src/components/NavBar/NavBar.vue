<template>
  <v-card
    height="100px"
    flat
    color="black"
    class="parent-nav"
    width="100%"
  >
    <v-bottom-nav
      :v-model="bottomNav"
      :value="true"
      absolute
      color="transparent"
      class="v-bottom-navi"
    >
      <v-btn
        color="transparent"
        flat
        value="home"
        @click="makeActive('home')"
        :class="bottomNav==='home' ? 'active' : ''"
      >
        <v-icon
          size="15px"
          :color="bottomNav==='home' ? '#5f9ea0' : 'white'"
          class="fas fa-home"
        >
        </v-icon>
        <span class="hidden-sm hidden-xs" >Inicio</span>
      </v-btn>

      <v-btn
        color="transparent"
        flat
        value="videos"
        @click="makeActive('videos')"
        :class="bottomNav==='videos' ? 'active' : ''"
      >
        <v-icon
          size="15px"
          :color="bottomNav==='videos' ? '#5f9ea0' : 'white'"
          class="fas fa-video"
        >
        </v-icon>
        <span class="hidden-sm hidden-xs">Videos</span>
      </v-btn>

      <v-btn
        color="transparent"
        flat
        value="contact"
        @click="makeActive('contact')"
        :class="bottomNav==='contact' ? 'active' : ''"
      >
        <v-icon
          size="15px"
          class="fas fa-envelope"
          :color="bottomNav==='contact' ? '#5f9ea0' : 'white'"
        >
        </v-icon>
        <span class="hidden-sm hidden-xs">Contacto</span>
      </v-btn>
    </v-bottom-nav>
  </v-card>
  <div class="headline text-xs-center pa-5">
    Active: {{ bottomNav }}
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  data () {
    return {
      bottomNav: 'home'
    }
  },
  methods: {
    makeActive: function (item){
      this.bottomNav = item;
    }
  }
};
</script>
<style scoped>
  .parent-nav{
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }
  .v-bottom-navi{
    height: fit-content;
  }
  .v-icon {
    margin: 5px;
  }
  .active{
    color: #5f9ea0 !important;
  }
</style>

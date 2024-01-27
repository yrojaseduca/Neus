<template class="CustomFooter">
  <v-footer
    color="black"
    height="auto"
  >
    <v-card
      class="flex"
      flat
      tile
      color="black"
    >
      <v-card-title class="teal">
        <strong class="subheading">Conecta con mis redes sociales!</strong>

        <v-spacer />

        <v-btn
          v-for="netButton in netButtons"
          :key="netButton.icon"
          class="mx-3"
          light
          icon
          :href="netButton.net"
          target="_blank"
        >
          <v-icon size="24px" color="#5f9ea0">
            {{ netButton.icon }}
          </v-icon>
        </v-btn>
      </v-card-title>

      <v-card-actions class="grey darken-3 justify-center">
        &copy;2014 — <strong>Neus González</strong>
      </v-card-actions>
    </v-card>
  </v-footer>
</template>

<script>

export default {
  name: 'CustomFooter',
  data: () => {
    return ({
      netButtons: [
        {
          'icon': 'fab fa-facebook',
          'net': 'https://www.instagram.com',
        },
        {
          'icon': 'fab fa-twitter',
          'net': 'https://www.instagram.com',
        },
        {
          'icon': 'fab fa-linkedin',
          'net': 'https://www.instagram.com',
        },
        {
          'icon': 'fab fa-instagram',
          'net': 'https://www.instagram.com',
        }
      ],
    });
  },
  methods: {
    goTo: function () {
      alert('Hello!')
    }
  }
};

</script>
<style scoped>
  .v-footer {
    justify-content: center;
  }
  strong {
    display: flex;
    justify-content: center;
    margin: 12px 0;
  }
</style>

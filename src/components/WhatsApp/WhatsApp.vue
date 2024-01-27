<template>
  <div class="WhatsApp">
    <v-btn
      v-for="netButton in netButtons"
      :key="netButton.icon"
      class="mx-3"
      light
      icon
      absolute
      top
      right
      fab
      :href="netButton.net"
      target="_blank"
    >
      <v-icon size="24px" color="#5f9ea0">
        {{ netButton.icon }}
      </v-icon>
    </v-btn>
  </div>
</template>

<script>
    export default {
        name: 'WhatsApp',
        data: () => {
        return ({
          netButtons: [
            {
              'icon': 'fab fa-whatsapp',
              'net': 'https://wa.me/607444947?text=hola! estoy interesada en un presupuesto!',
            },
          ],
        });
      },
    };
</script>
<style scoped>
  .WhatsApp {
    display: flex;
    justify-content: flex-end;
    position: fixed;
    right: 30px;
    bottom: 100px;
    z-index: 100;
  }
</style>

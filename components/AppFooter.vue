<template>
  <v-footer
    dark
    height="auto"
  >
    <v-card
      class="flex text-xs-center"
      flat
      tile
    >
      <v-card-text class="yellow darken-2">
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-3"
          dark
          icon
        >
          <v-icon size="24px">{{ icon }}</v-icon>
        </v-btn>
      </v-card-text>

      <v-card-text class="yellow darken-2 white--text text-xs-center">
        <strong>Vragen? Whatsapp ons nu: +31 6 84724899</strong>
      </v-card-text>

      <v-divider></v-divider>

      <v-card-actions class="grey darken-3 justify-center">
        &copy;2019 —<strong>&nbsp; Plyo</strong>
      </v-card-actions>
    </v-card>
  </v-footer>
</template>

<script>
  export default {
    data: () => ({
      icons: [
        'fa fa-facebook',
        'fa fa-twitter',
        'fa fa-linkedin',
        'fa fa-instagram'
      ]
    })
  }
</script>

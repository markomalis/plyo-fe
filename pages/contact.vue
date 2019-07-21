<template>
  <InlineSegment title="Contact">
    <blockquote class="blockquote">Plezier hebben in het trainen is bij ons een must maar het belangrijkste van alles is het bewust bezig zijn met je lichaam.
      Bij ons kun je kiezen uit de elementen kracht, conditie, mobiliteit en core.
      Deze combinatie van groepslessen zorgt ervoor dat je alle mogelijkheden van je lichaam (her)ontdekt en het optimale uit jouw bewegingespatroon haalt.
    </blockquote>
    <v-layout class="px-4" column justify-center>
      <v-flex class="sm12 md6 py-5">
        <v-img src="/kaart.png" aspect-ratio="1"></v-img>
      </v-flex>
      <v-flex class="sm12 md6 my-4">
        <v-layout class="" justify-center>
          <v-flex class="xs6">
            <div class="display-1 pb-3">Locatie</div>
            <div>Vlambloem 130</div>
            <div>3068JE, Ommoord</div>
          </v-flex>
          <v-flex class="xs6">
            <div class="display-1 pb-3">Contact</div>
            <div>Telefoon: 010 - 2071145</div>
            <div>Email: info@plyo.eu</div>
          </v-flex>
        </v-layout>
      </v-flex>
    </v-layout>
  </InlineSegment>
</template>

<script>
import InlineSegment from '~/components/InlineSegment.vue'

export default {
  components: {
    InlineSegment,
  }
}
</script>

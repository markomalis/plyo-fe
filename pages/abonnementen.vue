<template>
  <v-container fluid class="px-0 pt-0">
    <v-container>
      <InlineSegment title="Abonnementen">
        <v-layout
          wrap
        >
          <AboCard
            title="Plyo Plus"
            subscript="Onbeperkt + pilates voor een jaar"
            price="69"
            :features="plyoPlusFeatures"
            :action="{ title: 'Schrijf je in!', action: '/contact' }"
          />
          <AboCard
            title="Plyo Basis"
            subscript="Onbeperkt voor een jaar"
            price="59"
            :features="plyoBasicFeatures"
            :action="{ title: 'Schrijf je in!', action: '/contact' }"
          />
          <AboCard
            title="Plyo Students"
            subscript="Onbeperkt voor een jaar"
            price="39"
            :features="plyoStudentFeatures"
            :action="{ title: 'Schrijf je in!', action: '/contact' }"
          />
          <AboCard
            title="Plyo Kids"
            subscript="Onbeperkt voor een jaar"
            price="39"
            :action="{ title: 'Schrijf je in!', action: '/contact' }"
          />
          <AboCard
            title="Strippenkaart"
            subscript="8 lessen"
            price="75"
            :action="{ title: 'Koop een strippenkaart!', action: '/contact' }"
            :monthly="false"
          />
          <AboCard
            title="Proefles"
            subscript="Doe gratis een keer mee!"
            price="0"
            :action="{ title: 'Gratis proefles', action: '/contact' }"
            :monthly="false"
          />
        </v-layout>
      </InlineSegment>
    </v-container>
  </v-container>
</template>

<script>
import AboCard from '~/components/AboCard.vue'
import HomeCarousel from '~/components/HomeCarousel.vue'
import InlineSegment from '~/components/InlineSegment.vue'

export default {
  components: {
    AboCard,
    InlineSegment,
  },
  data: () => {
    return {
      plyoPlusFeatures: [
        'Onbeperkt',
        'Begeleiding',
        'Voedingsadvies',
        'Gratis intake',
        'Trainingsschema',
        'Pilates',
      ],
      plyoBasicFeatures: [
        'Onbeperkt',
        'Begeleiding',
        'Voedingsadvies',
        'Gratis intake',
        'Trainingsschema',
      ],
      plyoStudentFeatures: [
        'Onbeperkt',
        'Begeleiding',
        'Voedingsadvies',
      ],
    }
  }
}
</script>

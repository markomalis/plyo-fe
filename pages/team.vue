<template>
  <InlineSegment title="Team">
    <v-layout wrap justify-space-around>
      <ImageCard
        title="Salif Diao"
        subtitle="Coach"
        body_text="Een aantal keer een bootcamp gehad van deze toffe trainers. Het was echt killing!! Wat een energie heeft deze groep. Fantastisch dat zij dit zo goed kunnen overbrengen. Het gaf mij energie om er het maximale uit te halen en over mijn grenzen heen te stappen. Super bedankt Plyo!!"
        :action="{ title: 'Meer over Salif', href: '/team/salif' }"
      />
      <ImageCard
        title="Johnny Lopes Fortes"
        subtitle="Coach"
        body_text="Een aantal keer een bootcamp gehad van deze toffe trainers. Het was echt killing!! Wat een energie heeft deze groep. Fantastisch dat zij dit zo goed kunnen overbrengen. Het gaf mij energie om er het maximale uit te halen en over mijn grenzen heen te stappen. Super bedankt Plyo!!"
        :action="{ title: 'Meer over Johhny', href: '/team/johnny' }"
      />
      <ImageCard
        title="Lisanne"
        subtitle="Coach"
        body_text="Een aantal keer een bootcamp gehad van deze toffe trainers. Het was echt killing!! Wat een energie heeft deze groep. Fantastisch dat zij dit zo goed kunnen overbrengen. Het gaf mij energie om er het maximale uit te halen en over mijn grenzen heen te stappen. Super bedankt Plyo!!"
        :action="{ title: 'Meer over Lisanne', href: '/team/lisanne' }"
      />
    </v-layout>
  </InlineSegment>
</template>

<script>
import ImageCard from '~/components/ImageCard.vue'
import InlineSegment from '~/components/InlineSegment.vue'

export default {
  components: {
    ImageCard,
    InlineSegment,
  },
}
</script>

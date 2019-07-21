<template>
  <v-container fluid class="px-0 pt-0">
    <v-container fluid class="px-0 pt-0">
      <v-layout
        row
        justify-center
      >
        <v-flex
          xs12
        >
          <HomeCarousel />
        </v-flex>
      </v-layout>
    </v-container>
    <v-container>
      <p class="text-xs-center font-weight-bold font-italic display-2">Wil jij nu echt eens gaan werken aan sterker, fitter en leniger worden? We’ve got you covered.</p>
      <InlineSegment title="Abonnementen">
        <v-layout
          wrap
        >
          <AboCard
            title="Plyo Plus"
            subscript="Onbeperkt + pilates voor een jaar"
            price="69"
            :features="plyoPlusFeatures"
          />
          <AboCard
            title="Plyo Basis"
            subscript="Onbeperkt voor een jaar"
            price="59"
            :features="plyoBasicFeatures"
          />
          <AboCard
            title="Plyo Students"
            subscript="Onbeperkt voor een jaar"
            price="39"
            :features="plyoStudentFeatures"
          />
        </v-layout>
        <div class="text-xs-center">
          <v-btn
            round
            dark
            color="yellow darken-2 white--text"
            href="/abonnementen"
          >
            Meer informatie
          </v-btn>
        </div>
      </InlineSegment>
      <InlineSegment title="Groepslessen">
        <blockquote class="blockquote">Plezier hebben in het trainen is bij ons een must maar het belangrijkste van alles is het bewust bezig zijn met je lichaam.
          Bij ons kun je kiezen uit de elementen kracht, conditie, mobiliteit en core.
          Deze combinatie van groepslessen zorgt ervoor dat je alle mogelijkheden van je lichaam (her)ontdekt en het optimale uit jouw bewegingespatroon haalt.
        </blockquote>
        <div class="text-xs-center">
          <v-btn round color="yellow darken-2 white--text" dark>Gratis proefles</v-btn>
          <v-btn round color="yellow darken-2 white--text" dark>Meer informatie</v-btn>
        </div>
      </InlineSegment>
      <InlineSegment title="Ervaringen">
        <v-layout wrap justify-center>
          <ImageCard
            title="Demi"
            subtitle="Plyo workshops"
            body_text="Een aantal keer een bootcamp gehad van deze toffe trainers. Het was echt killing!! Wat een energie heeft deze groep. Fantastisch dat zij dit zo goed kunnen overbrengen. Het gaf mij energie om er het maximale uit te halen en over mijn grenzen heen te stappen. Super bedankt Plyo!!"
          />
          <ImageCard
            title="Demi"
            subtitle="Plyo workshops"
            body_text="Een aantal keer een bootcamp gehad van deze toffe trainers. Het was echt killing!! Wat een energie heeft deze groep. Fantastisch dat zij dit zo goed kunnen overbrengen. Het gaf mij energie om er het maximale uit te halen en over mijn grenzen heen te stappen. Super bedankt Plyo!!"
          />
          <ImageCard
            title="Demi"
            subtitle="Plyo workshops"
            body_text="Een aantal keer een bootcamp gehad van deze toffe trainers. Het was echt killing!! Wat een energie heeft deze groep. Fantastisch dat zij dit zo goed kunnen overbrengen. Het gaf mij energie om er het maximale uit te halen en over mijn grenzen heen te stappen. Super bedankt Plyo!!"
          />
          <ImageCard
            title="Demi"
            subtitle="Plyo workshops"
            body_text="Een aantal keer een bootcamp gehad van deze toffe trainers. Het was echt killing!! Wat een energie heeft deze groep. Fantastisch dat zij dit zo goed kunnen overbrengen. Het gaf mij energie om er het maximale uit te halen en over mijn grenzen heen te stappen. Super bedankt Plyo!!"
          />
        </v-layout>
      </InlineSegment>
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
          <div class="xs12 text-xs-center">
            <v-btn
              round
              dark
              color="yellow darken-2 white--text"
              href="/team"
            >
              Bekijk ons team
            </v-btn>
          </div>

      </InlineSegment>
    </v-container>
  </v-container>
</template>

<script>
import AboCard from '~/components/AboCard.vue'
import HomeCarousel from '~/components/HomeCarousel.vue'
import ImageCard from '~/components/ImageCard.vue'
import InlineSegment from '~/components/InlineSegment.vue'

export default {
  components: {
    AboCard,
    HomeCarousel,
    ImageCard,
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

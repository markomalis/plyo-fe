<template>
  <v-app>
    <v-toolbar
      class="grey darken-3"
      :clipped-left="clipped"
      fixed
      app
    >
      <!-- <v-toolbar-side-icon
        hidden-md-and-up
        @click="drawer = !drawer"
      /> -->
      <v-btn
        large
        icon
        href="/"
        class="home-button"
      >
        <img src="/plyo-logo.png" style="width='85px';" />
      </v-btn>
      <v-spacer />
      <ToolbarNavs
        :links="toolbarLinks"
      />
      <v-btn
        icon
        class="hidden-md-and-up"
        @click.stop="menuDrawer = false; menuDrawer = true"
      >
        <v-icon color="white">menu</v-icon>
      </v-btn>
    </v-toolbar>
    <NavDrawer :visible="menuDrawer" :links="toolbarLinks" />
    <v-content>
      <nuxt />
    </v-content>
    <AppFooter />
  </v-app>
</template>

<script>
import AppFooter from '~/components/AppFooter.vue'
import NavDrawer from '~/components/NavDrawer.vue'
import ToolbarNavs from '~/components/ToolbarNavs.vue'

export default {
  components: {
    AppFooter,
    NavDrawer,
    ToolbarNavs,
  },
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'bubble_chart',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      menuDrawer: false,
      title: 'Plyo',
      toolbarLinks: [
        { title: 'Abonnementen', href: '/abonnementen' },
        { title: 'Rooster', href: '/rooster' },
        { title: 'Team', href: '/team' },
        { title: 'Contact', href: '/contact' },
      ],
    }
  }
}
</script>

<style>
  .home-button {
    width: 85px !important;
  }
</style>

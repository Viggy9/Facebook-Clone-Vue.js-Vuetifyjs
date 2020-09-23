<template>
  <v-app>
    <v-app-bar
      fixed
      app
      dense
      flat
    >
    <v-row class="justify-center">
      <div class="d-flex justify-space-between">
      <v-btn text><v-icon>mdi-home</v-icon></v-btn>
            <v-btn text><v-icon>mdi-snapchat</v-icon></v-btn>
            <v-btn text><v-icon>mdi-clock</v-icon></v-btn>
            <v-btn text><v-icon>mdi-contacts</v-icon></v-btn>
            </div>

    </v-row>
  
    </v-app-bar>
    <v-main>
      <nuxt/>
    </v-main>
    <v-footer
      :absolute="!fixed"
      app
    >
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>

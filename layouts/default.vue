<template>
  <v-app dark>

    <v-main>
      <v-toolbar
      color="purple"
      dark
      >
      <v-toolbar-title>CLASSY</v-toolbar-title>

      <v-divider
        class="mx-4"
        vertical
      ></v-divider>

      <v-spacer></v-spacer>

      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn text>
          HOME
        </v-btn>

        <v-divider vertical></v-divider>

        <v-btn text>
          ABOUT
        </v-btn>

        <v-divider vertical></v-divider>

        <v-btn text>
          CONTACT
        </v-btn>

        <v-divider vertical></v-divider>
      </v-toolbar-items>

      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      </v-toolbar>
    
      <v-container
      w="100vh">
        <Nuxt />
      </v-container>
    </v-main>

   
    <v-footer :absolute="!fixed" app
    dark
    padless>
        <v-card
      class="flex"
      flat
      tile
    >
      <v-card-title class="purple">
    
        <v-spacer></v-spacer>

        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4"
          dark
          icon
        >
          <v-icon size="24px">
            {{ icon }}
          </v-icon>
        </v-btn>
      </v-card-title>

      <v-card-text class="py-2 white--text text-center">
        {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
      </v-card-text>
    </v-card>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
    }
  },
}
</script>

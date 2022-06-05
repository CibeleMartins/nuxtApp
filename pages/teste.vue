<template>
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
</template>

<script>
export default {
  name: 'TestePage',
}
</script>
 
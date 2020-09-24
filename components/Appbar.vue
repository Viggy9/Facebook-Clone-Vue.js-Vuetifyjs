<template>
  <v-app-bar dense clipped-left clipped-right color="#4267b2" dark app>
    <v-btn text><v-icon>mdi-facebook</v-icon></v-btn>
    <v-text-field append-icon="mdi-account-search" class="mt-6" label="Search" solo light dense></v-text-field>
    <v-spacer></v-spacer>
    <v-toolbar-items>
      <v-btn text class="text-none font-weight-bold">
        <v-icon left>mdi-face-profile</v-icon>Vignesh
      </v-btn>
      <v-btn text class="text-none font-weight-bold">Home</v-btn>
      <v-btn text class="text-none font-weight-bold">Create</v-btn>
    </v-toolbar-items>
    <v-toolbar-items>
      <v-btn icon>
        <v-icon color="white">mdi-home</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon color="white lighten-4">mdi-facebook-messenger</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon color="white lighten-4">mdi-snapchat</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon color="black lighten-4">mdi-help</v-icon>
      </v-btn>
    </v-toolbar-items>
  </v-app-bar>
</template>

<script>
export default {};
</script>


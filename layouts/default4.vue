<template>
<v-app  background-color="white">
    <v-system-bar dark color="indigo">
      <v-spacer></v-spacer>
      <v-icon>mdi-wifi-strength-4</v-icon>
      <v-icon>mdi-signal-cellular-outline</v-icon>
      <v-icon>mdi-battery</v-icon>
      <span>12:30</span>
  </v-system-bar>
<div>
  <v-app-bar
      color="primary"
      dense
      dark
      
    >
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>Destinations</v-toolbar-title>

      <v-spacer></v-spacer>

     

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
  </v-app-bar>
    </div>

  <!-- Sizes your content based upon application components -->
  <v-main>
    <v-content>
      <nuxt/>
    </v-content>
  </v-main>

 

</v-app>
</template>

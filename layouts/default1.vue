<template>
    <v-app>
      <v-system-bar
          color="blue-grey lighten-5"
          :height="height"
          :lights-out="lightsOut"
          :window="window"
        >
          <v-spacer></v-spacer>
          <v-icon style="color: #616161;">mdi-wifi-strength-4</v-icon>
          <v-icon style="color: #616161;">mdi-signal-cellular-outline</v-icon>
          <v-icon style="color: #616161;">mdi-battery</v-icon>
          <span style="color: #616161;">12:30</span>
        </v-system-bar>
<div>
  <v-app-bar
      color="grey darken-3"
      dense
      dark
    >
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      <v-toolbar-title>หน้าหลัก</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
      <v-menu
        left
        bottom
      >
        <template v-slot:activator="{ on, attrs }">
          <v-btn
            icon
            v-bind="attrs"
            v-on="on"
          >
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </template>
        <v-list>
          <v-list-item
            v-for="n in 5"
            :key="n"
            @click="() => {}"
          >
            <v-list-item-title>Option {{ n }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-app-bar>
  </div>
  <!-- Sizes your content based upon application components -->
  <v-main>
    <!-- Provides the application the proper gutter -->
    <v-content>
      <nuxt/>
    </v-content>
  </v-main>
  <v-footer
    dark
    padless
  >
    <v-card
      class="flex"
      flat
      tile
    >
      <v-card-title class="teal">
        <v-spacer></v-spacer>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4"
          dark
          icon
        >
          <v-icon size="24px">{{ icon }}</v-icon>
        </v-btn>
      </v-card-title>
      <v-card-text  class="py-2 white--text text-center" >
        {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</v-app>
</template>
<script>
export default {
  data:function(){
  return{
     icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
  }
  }
}
</script>
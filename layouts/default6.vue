<template>
  <v-app>
       <v-system-bar dark color="indigo">
      <v-spacer></v-spacer>
      <v-icon>mdi-wifi-strength-4</v-icon>
      <v-icon>mdi-signal-cellular-outline</v-icon>
      <v-icon>mdi-battery</v-icon>
      <span>12:30</span>
  </v-system-bar>
    <v-navigation-drawer v-model="drawer" app clipped>
      <lang-selector />
      <v-divider></v-divider>
      <v-list dense>
        <v-list-item v-for="item in items" :key="item.title" @click>
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <div>
      <v-app-bar color="blue " dense white>
        <v-btn icon>
          <v-icon>mdi-arrow-left</v-icon>
        </v-btn>
        <v-toolbar-title>Welcome</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn icon>
        </v-btn>
        <v-btn icon>
          <v-icon>mdi-magnify</v-icon>
        </v-btn>
        <v-menu left bottom>
          <template v-slot:activator="{ on, attrs }">
            <v-btn icon v-bind="attrs" v-on="on">
              <v-icon>mdi-dots-vertical</v-icon>
            </v-btn>
          </template>
        </v-menu>

      </v-app-bar>
      <v-tabs
    fixed-tabs
     background-color="primary"
    dark
  >
    <v-tab>
      SING UP
    </v-tab>
    <v-tab>
      SING IN
    </v-tab>
  </v-tabs>
       <nuxt/>
       
    </div>
    
    <!-- Sizes your content based upon application components -->
    <v-main>
      <!-- Provides the application the proper gutter -->
     
    </v-main>
    
    <v-footer app>
      <!-- -->
    </v-footer>
    
  </v-app>
</template>
<style>
#app {
    background: #ffffff;
}
</style>

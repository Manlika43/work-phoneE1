<template>
<center>
  <br>
   <v-card width="500" color="#1E88E5">
     <v-card-title-center>
      
      <h1>LOGIN</h1>
     </v-card-title-center>
     <v-card-text>
       <v-form>
         <v-text-field label="Username" 
          prepend-icon="mdi-account-circle"
          />
          <v-text-field 
            :type="showPassword ? 'text' : 'password'" 
            label="Password"
            prepend-icon="mdi-lock"
            :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"
            @click:append="showPassword = !showPassword"
          />
       </v-form>
     </v-card-text>
     <v-card-actions>
    <nuxt-link to="\register"><v-btn class="ma-2" tile color="#00695C" dark>REGISTER</v-btn></nuxt-link>
    <v-spacer></v-spacer>
   <v-btn class="ma-2" tile color="light-blue darken-3" dark>LOGIN</v-btn>
    </v-btn>
    </v-btn>
  </v-card-actions>
   </v-card>
   </center>
</template>
<script>
export default {
  name: 'App',
  data () {
    return {
      showPassword: false
    }
  }
}
</script>


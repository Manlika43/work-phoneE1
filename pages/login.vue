<template>

   <v-card>
     <v-card-title>
       <h1>Login</h1>
     </v-card-title>
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
      
  
  <v-card-actions>
       <nuxt-link to="/register">
    <v-btn class="ma-2" tile color="green darken-4" dark>REGISTER</v-btn>
    </nuxt-link>
     <v-spacer></v-spacer>
     
     <v-btn class="ma-2" tile color="light-blue darken-3" dark>LOGIN</v-btn>
    
 </v-card-actions>

       
     </v-card-text>
   </v-card>
   
 
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
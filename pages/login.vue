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
       </v-form>
       <v-form>
         <v-text-field label="Password" prepend-icon="lock" append-icon="visibility_off"/>
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
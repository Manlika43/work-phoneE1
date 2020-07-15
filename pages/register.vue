<template>
<center>
  <br>
   <v-card width="400" color="blue darken-4" >
     <v-card-title>
      
      <h1>REGISTER</h1>
     </v-card-title>
     <v-card-text>
       <v-form>
         <v-text-field label="Username" 
          prepend-icon="mdi-account-circle"
          />
          <v-text-field label="Password" 
          prepend-icon="mdi-lock"
          />
           <v-text-field label="Email" 
          prepend-icon="email"
          />
           <v-text-field label="Tell" 
          prepend-icon="perm_phone_msg"
          />
       </v-form>
     </v-card-text>
     <v-card-actions>
    <v-btn class="ma-2" tile color="red darken-3" dark>REGISTER</v-btn>
    <v-spacer></v-spacer>
   <nuxt-link to="login"><v-btn class="ma-2" tile color="light-blue darken-3" dark>CANCEL</v-btn></nuxt-link>
    </v-btn>
    </v-btn>
  </v-card-actions>
   </v-card>
   </center>
</template>
<script>


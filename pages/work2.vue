<template>
<div class="container"><br>
     <center><v-list-item-avatar style="width:90px; height:90px;">
            <img src="images/pla.jpg" width="100%"/>
          </v-list-item-avatar></center>

          <v-card
    class="mx-auto"
    max-width="344"
  >
    <v-card-text>
      <v-form>
    <v-container>
      <v-row>

        <v-col cols="12" sm="4">
          <v-text-field
            label="Username"
            single-line
            outlined
          ></v-text-field>
        </v-col>

         <v-col cols="12" sm="6" style="margin-top:-30px;">
          <v-text-field
            label="Password"
            single-line
            outlined
          ></v-text-field>
        </v-col>
        

      </v-row>
       <v-checkbox
          v-model="absolute"
          label="remember me"
          style="margin-top:-30px;"
        >
      
        </v-checkbox>
         <p style="margin-top:-45px; margin-left:170px;">Forgot Password</p>
       
    </v-container>
  </v-form>
  
    </v-card-text>
    <v-card-actions>
      <v-btn
        text
        color="deep-purple accent-4"
      >
      
       <center><nuxt-link to="../work3"> <v-btn color="#283593" dark style="width:300px; margin-top:-40px;">SIGN IN</v-btn></nuxt-link></center>
      </v-btn>
    </v-card-actions>
  </v-card>
          </div>
          
</template>
<script>
export default {
   layout : "work_2",
}
</script>
 
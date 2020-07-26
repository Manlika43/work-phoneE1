<template>
  <div>
    <h1>HELLO {{ first }}age:{{std}} </h1>
     <v-text-field
            v-model="first1"
            label="กรุณากรอกชื่อ"
            placeholder="กรุณากรอกชื่อของท่าน"
            outlined
            shaped
          ></v-text-field>
           <v-col cols="12" sm="6" md="3">
          <v-text-field
            label="Solo"
            placeholder="กรุณาใส่ชื่อเล่น"
            solo
          ></v-text-field>
        </v-col>
         <v-col cols="12" sm="6">
          <v-text-field
            label="Email"
            single-line
          ></v-text-field>
        </v-col>
         <v-col cols="12" sm="6">
          <v-text-field
            v-model="last"
            label="กรอกเบอร์โทรศัพท์"
            filled
            shaped
          ></v-text-field>
        </v-col>
  </div>
  
</template>
<script>
export default {
  data:function(){
    return{
     name:"alongkorn",
     age:45,
     dep:"information  technology",
     first:"chaiyaphum"

    }
  }
}
</script>
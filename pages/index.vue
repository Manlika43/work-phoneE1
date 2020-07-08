<template>
  <div>
    <h1 v-t="'สมุดบันทึกกิจกรรม'" />
    <div class="my-2">
            <nuxt-link to="/menu">
            <div class="text-center">
                 <v-btn rounded color="error" dark>ไปสู่เมนูหลัก</v-btn>
            </div>
             </nuxt-link>
              <nuxt-link to="/Ex01">
            <div class="text-center">
                 <v-btn rounded color="error" dark>กลับหน้าล็อกอิน</v-btn>
            </div>
             </nuxt-link>
          </div>
  </div>
</template>

<template>
  <v-app>
    <v-container>
      <div class="text-center pt-5 pb-4">
        <img src="https://image.freepik.com/free-vector/people-holding-heart-hand-icons_53876-66152.jpg" width="200">
        </img>
        <h3>Masuk ke Karto</h3>
      </div>
      <v-card outlined class="text-center pt-5 mx-16">
        <v-btn width="305" outlined color="blue darken-3">
          <img class="mr-3" width="17" src="https://image.flaticon.com/icons/svg/2702/2702602.svg">
          Masuk menggunakan Google
        </v-btn>
        <p class="mt-5">atau</p>
        <v-text-field class="mx-3 mt-6" outlined dense label="Nama pengguna atau alamat email"></v-text-field>
        <v-text-field class="mx-3" type="password" outlined dense label="Kata sandi"></v-text-field>
        <v-btn width="305" class="mb-3" color="primary" >Masuk</v-btn>
      </v-card>
    </v-container>
  </v-app>
</template>

<script>
  export default {
    layout: 'empty'
  }
</script>
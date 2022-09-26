<template>
    <div>
        <v-toolbar short>
            <n-link to="/morinanapost1" class="text-decoration-none">
                <v-btn icon>
                    <v-icon>mdi-arrow-left</v-icon>
                </v-btn>
            </n-link>
            <v-toolbar-title>
                <h5>Kaori Menderita Kanker Stadium 3</h5>
            </v-toolbar-title>
        </v-toolbar>
        <v-container>
            <div class="ml-3 mt-5 d-flex">
                <v-avatar size="62">
                    <v-img src="https://marucco-lino.com/wp-content/uploads/2019/06/%E6%A3%AE%E4%B8%83%E8%8F%9C.jpg"></v-img>
                </v-avatar>
                <div class="flex-column ml-3">
                    <h4 class="mb-1">MoriNana<v-icon color="primary" small class="mb-1 ml-2 mr-5">mdi-check-circle</v-icon></h4>
                    <p class="font-weight-light">nanamori</p>
                </div>
                <p class="ml-10">3h yang lalu</p>
            </div>
            <div class="text-center">
                <img height="182" src="https://api.duniagames.co.id/api/content/upload/file/6356485281585889003.jpg">
            </div>
            <p class="text-justify caption">Terimakasih atas donasinya untuk pengobatan Kaori, yang sekarang sudah terkumpul sebanyak Rp200.000.000. Semoga dengan donasi yang sudah terkumpul bisa memberikan kemudahan pengobatan Kaori, dan semoga Allah memberikan kesembuhan pada Kaori.</p>
        </v-container>
        <n-link to="/tambahkabarterbaru" class="text-decoration-none">
            <v-btn block tile color="orange accent">Tambah Kabar Terbaru</v-btn>
        </n-link>
    </div>
</template>
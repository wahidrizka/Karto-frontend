<template>
    <div>
        <v-toolbar short dense class="mb-3">
            <n-link to="/lieryrosepost1" class="text-decoration-none">
                <v-btn icon>
                    <v-icon>mdi-arrow-left</v-icon>
                </v-btn>
            </n-link>
            <v-toolbar-title>
                <h5>Kontak dan Lokasi Penggalang</h5>
            </v-toolbar-title>
        </v-toolbar>
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3953.3062627381396!2d110.394498114703!3d-7.757306979075844!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e7a59a14a4055c5%3A0xcb3932037376c617!2sBalai%20Desa%20Condongcatur!5e0!3m2!1sen!2sid!4v1597643352331!5m2!1sen!2sid" width="340" height="500" frameborder="0" style="border:0;" aria-hidden="false" tabindex="0"></iframe>
        <v-container class="d-flex">
            <v-icon large color="primary">
                mdi-home-circle
            </v-icon>
            <h4 class="ml-2 mt-1">Condong Catur, Sleman, Yogyakarta</h4>
        </v-container>
        <div class="d-flex justify-space-between">
            <v-btn outlined color="primary">
                Kontak Penggalang
            </v-btn>
            <v-btn color="primary">
                Buka Map
            </v-btn>
        </div>
    </div>
</template>
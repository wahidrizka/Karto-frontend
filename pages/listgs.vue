<template>
    <v-tabs fixed-tabs>
        <v-tab key="aktif">Aktif</v-tab>
        <v-tab key="selesai">Selesai</v-tab>
        <v-tab-item key="aktif">
            <v-container>
                <v-card class="pl-5 pa-3">
                    <div>
                        <p class="caption"><v-icon class="mr-3" small>mdi-timer-outline</v-icon>Tersisa 16 Hari</p>
                        <h4>Gerakan Mahasiswa Anti-Hoax Yogyakarta</h4>
                        <div class="mt-2 mr-5">
                        <v-progress-linear color="blue" height="8" rounded value="80"></v-progress-linear>
                        <p class="text-caption">Relawan: 32 dari 140</p>
                        <v-progress-linear color="blue" height="8" rounded value="83.77"></v-progress-linear>
                        <p class="text-caption">Donasi: Rp8.337.000 / Rp10.000.000 </p>
                        </div>
                    </div>
                </v-card>
            </v-container>
            <v-container>
                <v-card class="pl-5 pa-3">
                    <div>
                        <p class="caption"><v-icon class="mr-3" small>mdi-timer-outline</v-icon>Tersisa 16 Hari</p>
                        <h4>Aksi Tebar Daging Qurban Melintasi Batas</h4>
                        <div class="mt-2 mr-5">
                            <v-progress-linear color="blue" height="8" rounded value="83.77"></v-progress-linear>
                            <p class="text-caption">Donasi: Rp8.337.000 / Rp10.000.000 </p>
                            <v-progress-linear color="blue" height="8" rounded value="83.77"></v-progress-linear>
                            <p class="text-caption">Daging: 31kg / 100kg</p>
                        </div>
                    </div>
                </v-card>
            </v-container>
        </v-tab-item>
        <v-tab-item key="selesai">
        </v-tab-item>
    </v-tabs>
</template>
<template>
    <v-tabs color fixed-tabs>
        <v-tab key="aktif">Aktif</v-tab>
        <v-tab key="selesai">Selesai</v-tab>
        <v-tab-item key="aktif">
            <v-container>
                <v-card class="pl-5 pa-3">
                    <div>
                        <p class="caption"><v-icon class="mr-3" small>mdi-timer-outline</v-icon>Tersisa 13 Hari</p>
                        <h4>Kaori Menderita Kangker Stadium 3</h4>
                        <div class="d-flex justify-space-between">
                            <p class="mt-5 caption"><v-icon class="mr-3 mb-1" small>mdi-thumb-up</v-icon>1,1 Ribu Pendukung</p>
                            <v-icon class="mr-3">mdi-share</v-icon>
                        </div>
                    </div>
                </v-card>
            </v-container>
            <v-container>
                <v-card class="pl-5 pa-3">
                    <div>
                        <p class="caption"><v-icon class="mr-3" small>mdi-timer-outline</v-icon>Tersisa 13 Hari</p>
                        <h4>BisaMakanDaging - Berbagi Daging Untuk Dhuafa</h4>
                        <div class="d-flex justify-space-between">
                            <p class="mt-5 caption"><v-icon class="mr-3 mb-1" small>mdi-thumb-up</v-icon>1,1 Ribu Pendukung</p>
                            <v-icon class="mr-3">mdi-share</v-icon>
                        </div>
                    </div>
                </v-card>
            </v-container>
        </v-tab-item>
        <v-tab-item key="selesai">
        </v-tab-item>
    </v-tabs>
</template>
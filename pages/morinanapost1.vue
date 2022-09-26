<template>
    <div>
        <v-toolbar short>
            <n-link to="/exploregb" class="text-decoration-none">
                <v-btn icon>
                    <v-icon>mdi-arrow-left</v-icon>
                </v-btn>
            </n-link>
            <v-toolbar-title>
                <h5>Postingan MoriNana</h5>
            </v-toolbar-title>
        </v-toolbar>
        <div class="ml-3 mt-5 d-flex">
            <v-avatar size="62">
                <v-img src="https://marucco-lino.com/wp-content/uploads/2019/06/%E6%A3%AE%E4%B8%83%E8%8F%9C.jpg"></v-img>
            </v-avatar>
            <div class="flex-column ml-3">
                <h4 class="mb-1">MoriNana<v-icon color="primary" small class="mb-1 ml-2">mdi-check-circle</v-icon></h4>
                <p class="font-weight-light">nanamori</p>
            </div>
        </div>
        <v-carousel height="250"
            :show-arrows="false"
            delimiter-icon=mdi-circle-medium>
            <v-carousel-item
                src="https://i1.wp.com/newsrush.in/wp-content/uploads/2020/07/doctors-day-2020-a-medic-shares-how-hard-lockdown-has-been-for-cancer-patients.jpg?w=1020&ssl=1">
            </v-carousel-item>
            <v-carousel-item
                src="https://i1.wp.com/newsrush.in/wp-content/uploads/2020/07/doctors-day-2020-a-medic-shares-how-hard-lockdown-has-been-for-cancer-patients.jpg?w=1020&ssl=1">
            </v-carousel-item>
            <v-carousel-item
                src="https://i1.wp.com/newsrush.in/wp-content/uploads/2020/07/doctors-day-2020-a-medic-shares-how-hard-lockdown-has-been-for-cancer-patients.jpg?w=1020&ssl=1">
            </v-carousel-item>
            <v-carousel-item
                src="https://i1.wp.com/newsrush.in/wp-content/uploads/2020/07/doctors-day-2020-a-medic-shares-how-hard-lockdown-has-been-for-cancer-patients.jpg?w=1020&ssl=1">
            </v-carousel-item>
            <v-carousel-item
                src="https://i1.wp.com/newsrush.in/wp-content/uploads/2020/07/doctors-day-2020-a-medic-shares-how-hard-lockdown-has-been-for-cancer-patients.jpg?w=1020&ssl=1">
            </v-carousel-item>
        </v-carousel>
        <div class="d-flex mt-1 justify-space-around">
            <div class="d-flex">
                <v-btn disabled icon color="primary">
                    <v-icon>mdi-progress-clock</v-icon>
                </v-btn>
                <p class="caption font-weight-bold mt-2">13 Hari Lagi</p>
            </div>
            <div class="d-flex">
                <v-btn disabled icon color="primary">
                    <v-icon>mdi-thumb-up-outline</v-icon>
                </v-btn>
                <p class="caption font-weight-bold mt-2">1,1 Ribu Mendukung</p>
            </div>
            <div>
                <v-btn icon color="primary">
                    <v-icon>mdi-share</v-icon>
                </v-btn>
            </div>
        </div>
        <h3>Kaori Menderita Kanker Stadium 3</h3>
        <h4 class="mt-2 font-weight-bold">Bantuan Dibutuhkan</h4>
        <v-card class="my-2">
            <div class="d-flex justify-space-between pa-2 pt-4">
                <p><v-icon color="primary">mdi-cash</v-icon> Uang</p>
                <v-btn class="px-10" color="primary" small @click="dialoginputnominal = true">Donasi</v-btn>
            </div>
        </v-card>
        <v-dialog v-model="dialoginputnominal" persistent>
            <v-card>
                <v-toolbar dense flat>
                    <v-btn icon @click="dialoginputnominal = false">
                        <v-icon>mdi-close</v-icon>
                    </v-btn>
                    <v-toolbar-title>
                        <h4>Jumlah Donasi</h4>
                    </v-toolbar-title>
                </v-toolbar>
                <v-container class="text-center">
                    <v-text-field color="blue accent" prefix="Rp" dense outlined label="Masukan jumlah donasi">
                    </v-text-field>
                </v-container>
                <v-btn @click="dialogrekeninglist = true" block tile color="blue accent">Lanjutkan</v-btn>
            </v-card>
        </v-dialog>
        <v-dialog v-model="dialogrekeninglist" persistent>
            <v-card>
                <v-toolbar dense flat>
                    <v-btn icon @click="dialogrekeninglist = false">
                        <v-icon>mdi-arrow-left</v-icon>
                    </v-btn>
                    <v-toolbar-title>
                        <h4>Pilih Bank</h4>
                    </v-toolbar-title>
                </v-toolbar>
                <v-container>
                    <v-list dense>
                        <v-list-item-group color="blue accent">
                            <v-list-item>
                                <div class="d-flex pa-3">
                                    <img width="70" height="50" src="https://1.bp.blogspot.com/-nYGeWq_cRBc/UmI9R592JpI/AAAAAAAADAI/QPAKTHg7cUk/s350/Logo-Bank-BRI-transparent-background.png">
                                    <div>
                                        <h5 class="ml-5 font-weight-regular">Transfer Lewat</h5>
                                        <h5 class="ml-5">Bank Rakyat Indonesia</h5>
                                    </div>
                                </div>
                            </v-list-item>
                            <v-divider></v-divider>
                            <v-list-item>
                                <div class="d-flex pa-3">
                                    <img width="70" height="50" src="https://i.pinimg.com/originals/b2/66/1a/b2661a071d61614b6c7201a60fc806e9.jpg">
                                    <div>
                                        <h5 class="ml-5 font-weight-regular">Transfer Lewat</h5>
                                        <h5 class="ml-5">Bank Negara Indonesia</h5>
                                    </div>
                                </div>
                            </v-list-item>
                            <v-divider></v-divider>
                            <v-list-item>
                                <div class="d-flex pa-3">
                                    <img width="70" height="50" src="https://cdn.freebiesupply.com/logos/thumbs/2x/bca-bank-central-asia-logo.png">
                                    <div>
                                        <h5 class="ml-5 font-weight-regular">Transfer Lewat</h5>
                                        <h5 class="ml-5">Bank Central Asia</h5>
                                    </div>
                                </div>
                            </v-list-item>
                            <v-divider></v-divider>
                            <v-list-item>
                                <div class="d-flex pa-3">
                                    <img width="70" height="50" src="https://img2.pngio.com/bank-mandiri-png-7-png-image-bank-mandiri-png-1007_580.png">
                                    <div>
                                        <h5 class="ml-5 font-weight-regular">Transfer Lewat</h5>
                                        <h5 class="ml-5">Bank Mandiri</h5>
                                    </div>
                                </div>
                            </v-list-item>
                            <v-divider></v-divider>
                            <v-list-item>
                                <div class="d-flex pa-3">
                                    <img width="70" height="50" src="https://www.donasi.tendavisi.org/wp-content/uploads/2019/12/Bank-Muamalat-New.png">
                                    <div>
                                        <h5 class="ml-5 font-weight-regular">Transfer Lewat</h5>
                                        <h5 class="ml-5">Bank Muamalat</h5>
                                    </div>
                                </div>
                            </v-list-item>
                            <v-divider></v-divider>
                        </v-list-item-group>
                    </v-list>
                </v-container>
                <v-btn @click="dialogdetaildonasi = true" block tile color="blue accent">Lanjutkan</v-btn>
            </v-card>
        </v-dialog>
        <v-dialog v-model="dialogdetaildonasi" persistent>
            <v-card>
                <v-toolbar dense flat>
                    <v-btn icon @click="dialogdetaildonasi = false">
                        <v-icon>mdi-arrow-left</v-icon>
                    </v-btn>
                    <v-toolbar-title>
                        <h4>Konfirmasi Transfer</h4>
                    </v-toolbar-title>
                </v-toolbar>
                <v-container>
                    <div>
                        <h5>Jumlah Transfer</h5>
                        <v-text-field prefix="Rp" readonly outlined dense value="inijumlahdonasi"></v-text-field>
                    </div>
                    <div>
                        <h5>Rekening Tujuan</h5>
                        <v-text-field prefix="inikodebank" readonly outlined dense value="034 888 9987"></v-text-field>
                    </div>
                </v-container>
                <v-btn @click="dialogdetaildonasi = false, dialoginputnominal = false, dialogrekeninglist = false" block tile color="blue accent">Lanjutkan</v-btn>
            </v-card>
        </v-dialog>
        <h4 class="my-3">Donasi Terkumpul</h4>
        <v-progress-linear rounded color="primary" height="10" value="83"></v-progress-linear>
        <p class="caption font-weight-bold">Uang : Rp 8.337.000 / Rp 10.000.000</p>
        <h4>Cerita Penggalang :</h4>
        <p class="text-justify">Penyakit tersebut membuat tubuh Kaori menjadi lemah dan dirinya kesulitan untuk berdiri hingga akhirnya ia harus dirawat di rumah sakit selama beberapa hari. </p>
        <p class="text-justify">Penyakit yang dialami oleh Kaori telah dijelaskan langsung oleh dokter, bahwa Kaori mengidap penyakit kanker yang mematikan, serta penyakit sumsum tulang.</p>
        <div class="mx-auto text-center mb-3">
            <iframe
                width="300"
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d31634.25427735431!2d110.72300377063273!3d-7.6528198451432825!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0xc75de9ebb0022598!2sSD%20Negeri%20Juwiring!5e0!3m2!1sen!2sid!4v1597895870400!5m2!1sen!2sid" 
                frameborder="0" 
                style="border:0;" 
                allowfullscreen="" 
                aria-hidden="false">
            </iframe>
        </div>
        <div>
            <v-badge text inline content="1">
                <h4>Kabar Terbaru</h4>
            </v-badge>
            <n-link to="/kabarterbaru" class="text-decoration-none">
            <v-card class="mx-auto pt-2 mt-1">
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
                    <p class="text-justify caption">Terimakasih atas donasinya untuk pengobatan Kaori...</p>
                </v-container>
            </v-card>
            </n-link>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            dialoginputnominal: false,
            dialogrekeninglist: false,
            dialogdetaildonasi: false,
        }
    }
}
</script>
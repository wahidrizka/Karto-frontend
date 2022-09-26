<template>
    <div>
        <v-toolbar short>
            <n-link to="/exploregs" class="text-decoration-none">
                <v-btn icon>
                    <v-icon>mdi-arrow-left</v-icon>
                </v-btn>
            </n-link>
            <v-toolbar-title>
                <h5>Postingan AFfdn</h5>
            </v-toolbar-title>
        </v-toolbar>
        <div class="ml-3 mt-5 d-flex">
            <v-avatar size="62">
                <v-img src="https://pro2-bar-s3-cdn-cf1.myportfolio.com/8a80f68b42f1d81272f688d4709074fc/cd049b08-eded-4033-a61a-b9ba8983c3af_rwc_0x0x404x316x404.png?h=7994bca2229cd990b13bfb946f4e4bb3"></v-img>
            </v-avatar>
            <div class="flex-column ml-3">
                <h4 class="mb-1">AFfdn<v-icon color="primary" small class="mb-1 ml-2">mdi-check-circle</v-icon></h4>
                <p class="font-weight-light">affdn</p>
            </div>
        </div>
        <v-carousel height="auto"
            :show-arrows="false"
            delimiter-icon=mdi-circle-medium>
            <v-carousel-item>
                <img height="200" src="https://s3-alpha-sig.figma.com/img/1776/d1e6/f462175ee5617002577a57f7c85fa55d?Expires=1598227200&Signature=MzYUqCkDeDnVmUTtbQxE~ajG0oF3XcDC9TqGhQM9fWzL2xtVljpP5kzVc6fS80wO~rdehl8q0cbAYpc-5JfATQN5G11pDxxeZQUUAlzog3HL4v6g~CW-e76z-iZ00pQ5mqjolEll5kQ3A7cWBF0Aah8GKY66tRsuBJecw6dx1rUrx-zjiN04q6olIINMn7YxEi3zYREeblPKge~8VkEiHu~DvY0t7yDqMnGRpK4O1DC5UrwoJ--JRcf3nhn0jq1BZAAwMdaBl8wkx3aviewMfQZ1~p2aTIp5N5aS8~9LZNn-N1gsBBR5QLiCRXjd~msMFYwqzaJAwCYTGYvdUZWXLw__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
            </v-carousel-item>
            <v-carousel-item>
                <img height="200" src="https://s3-alpha-sig.figma.com/img/1776/d1e6/f462175ee5617002577a57f7c85fa55d?Expires=1598227200&Signature=MzYUqCkDeDnVmUTtbQxE~ajG0oF3XcDC9TqGhQM9fWzL2xtVljpP5kzVc6fS80wO~rdehl8q0cbAYpc-5JfATQN5G11pDxxeZQUUAlzog3HL4v6g~CW-e76z-iZ00pQ5mqjolEll5kQ3A7cWBF0Aah8GKY66tRsuBJecw6dx1rUrx-zjiN04q6olIINMn7YxEi3zYREeblPKge~8VkEiHu~DvY0t7yDqMnGRpK4O1DC5UrwoJ--JRcf3nhn0jq1BZAAwMdaBl8wkx3aviewMfQZ1~p2aTIp5N5aS8~9LZNn-N1gsBBR5QLiCRXjd~msMFYwqzaJAwCYTGYvdUZWXLw__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
            </v-carousel-item>
            <v-carousel-item>
                <img height="200" src="https://s3-alpha-sig.figma.com/img/1776/d1e6/f462175ee5617002577a57f7c85fa55d?Expires=1598227200&Signature=MzYUqCkDeDnVmUTtbQxE~ajG0oF3XcDC9TqGhQM9fWzL2xtVljpP5kzVc6fS80wO~rdehl8q0cbAYpc-5JfATQN5G11pDxxeZQUUAlzog3HL4v6g~CW-e76z-iZ00pQ5mqjolEll5kQ3A7cWBF0Aah8GKY66tRsuBJecw6dx1rUrx-zjiN04q6olIINMn7YxEi3zYREeblPKge~8VkEiHu~DvY0t7yDqMnGRpK4O1DC5UrwoJ--JRcf3nhn0jq1BZAAwMdaBl8wkx3aviewMfQZ1~p2aTIp5N5aS8~9LZNn-N1gsBBR5QLiCRXjd~msMFYwqzaJAwCYTGYvdUZWXLw__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
            </v-carousel-item>
        </v-carousel>
        <div class="d-flex mt-1 justify-space-around">
            <div class="d-flex">
                <v-btn disabled icon color="primary">
                    <v-icon>mdi-progress-clock</v-icon>
                </v-btn>
                <p class="caption font-weight-bold mt-2">16 Hari Lagi</p>
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
        <h3>Aksi Tebar Daging Kurban Melintasi Batas</h3>
        <v-badge class="mt-4" text inline content="32">
            <h4>Relawan Terdaftar</h4>
        </v-badge>
        <div class="d-flex justify-space-between">
            <v-avatar size="33">
                <img src="https://1.bp.blogspot.com/-0k7hXCt2b_M/XeqVbW1E_QI/AAAAAAABCuQ/CPi_wNmesGcojb0_xDckOAO-6TBNBX9YgCLcBGAsYHQ/s1600/413eq4r3.jpg">
            </v-avatar>
            <v-avatar size="33">
                <img src="https://steamuserimages-a.akamaihd.net/ugc/149011680355880328/B370950862F02D196E12E7DFC1DAE8BA997D9805/">
            </v-avatar>
            <v-avatar size="33">
                <img src="https://i1.wp.com/metro.co.uk/wp-content/uploads/2019/08/GettyImages-105110849-e1565444355445.jpg?quality=90&strip=all&zoom=1&resize=644%2C538&ssl=1">
            </v-avatar>
            <v-avatar size="33">
                <img src="https://m.media-amazon.com/images/M/MV5BMjExNzA4MDYxN15BMl5BanBnXkFtZTcwOTI1MDAxOQ@@._V1_UY317_CR7,0,214,317_AL_.jpg">
            </v-avatar>
            <v-avatar size="33">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQAchV5Pp5k-_3LwwYcN_z_0wH90WYIFfGjXQ&usqp=CAU">
            </v-avatar>
            <v-avatar size="33">
                <img src="https://pbs.twimg.com/media/EYyTN1YUMAA7E1x.jpg">
            </v-avatar>
            <v-avatar size="33">
                <img src="https://cdn1-production-images-kly.akamaized.net/ostt0KnD3HVkharuNlk9LMfMYH8=/640x640/smart/filters:quality(75):strip_icc():format(jpeg)/kly-media-production/medias/709259/original/Tyrese-Gibson-160714.gif">
            </v-avatar>
            <v-avatar color="primary" size="33">
                <span class="caption white--text">25+</span>
            </v-avatar>
        </div>

        <h4 class="mt-5">Donasi Terkumpul</h4>
        <v-progress-linear rounded color="primary" height="10" value="83"></v-progress-linear>
        <p class="caption font-weight-bold">Uang : Rp 8.337.000 / Rp 10.000.000</p>
        <v-progress-linear color="primary" height="10" value="31" rounded></v-progress-linear>
        <p class="caption font-weight-bold">Daging : 31 Kg / 100 Kg</p>
        <h4 class="mt-4">Deskripsi :</h4>
        <p class="text-justify">Pembagian dibagikan secara door to door namun jika warga mengambil secara langsung dengan syarat melaksanakan protokol kesehatan Covid-19. Kami juga sediakan tempat cuci tangan, sebelum mengambil daging kurban, kami persilakan untuk cuci tangan dulu, kalau tidak pakai masker kami tidak akan kasih daging kurbannya.</p>
        <h4>Detail Kegiatan</h4>
        <div>
            <p><v-icon class="mr-2">mdi-calendar</v-icon>10-31 Agustus</p>
            <p><v-icon class="mr-2">mdi-map-marker</v-icon>Condong Catur</p>
            <p><v-icon class="mr-2">mdi-briefcase-variant-outline</v-icon>5 Peran Tersedia</p>
            <p><v-icon class="mr-2">mdi-face-outline</v-icon>13 Teman Kamu Juga Berpartisipasi</p>
        </div>
        <div class="mx-auto text-center mb-3">
            <iframe
                width="300"
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3953.3062627381473!2d110.39449811437623!3d-7.757306979075043!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e7a59a14a4055c5%3A0xcb3932037376c617!2sBalai%20Desa%20Condongcatur!5e0!3m2!1sen!2sid!4v1597895670963!5m2!1sen!2sid" 
                frameborder="0" 
                style="border:0;" 
                allowfullscreen="" 
                aria-hidden="false">
            </iframe>
        </div>
        <div class="mb-3">
            <v-badge text inline content="0">
                <h4>Kabar Terbaru</h4>
            </v-badge>
            <v-card height="100" class="text-center mx-auto">
                <p>Belum ada kabar terbaru</p>
            </v-card>
        </div>
        <v-toolbar height="90" rounded>
            <v-row justify="space-around" class="my-2">
                <v-btn color="primary" class="ma-2" @click="dialog = true">
                    Gabung Relawan
                </v-btn>
                <v-btn color="primary" class="ma-2" @click="dialog2 = true">
                    Donasi
                </v-btn>
                <v-dialog v-model="dialog" persistent>
                    <v-card>
                        <v-toolbar dense flat>
                            <v-btn icon @click="dialog = false">
                                <v-icon>mdi-close</v-icon>
                            </v-btn>
                            <v-toolbar-title>
                                <h4>Peran Dalam Kegiatan</h4>
                            </v-toolbar-title>
                        </v-toolbar>
                        <v-container>
                            <h4 class="font-weight-regular">Berikut adalah peran tersedia yang dapat kamu ambil di kegiatan ini.</h4>
                        </v-container>
                        <v-divider></v-divider>
                        <v-container>
                            <v-btn class="my-3" color="blue accent" width="100%" v-for="job in jobs" :key="job.text" @click="dialog=false,dialogjoin=true" >{{job.text}}</v-btn>   
                        </v-container>    
                    </v-card>
                </v-dialog>
                <v-dialog v-model="dialog2" max-width="600px">
                    <v-card class="pa-2">
                        <v-card-title>Pilih Tipe Donasi</v-card-title>
                        <v-card-text>Selain menjadi volunteer, kamu juga dapat ikut mendukung kegiatan ini dengan menjadi donatur.</v-card-text>
                        <div class="pa-3">
                            <v-btn class="mb-2" color="primary" width="100%" @click="dialoginputnominal=true, dialog2=false" >Uang</v-btn>
                            <br>
                            <v-btn class="my-2" color="primary" width="100%" @click="dialogdonasidaging=true, dialog2=false" >Daging</v-btn>
                        </div>    
                    </v-card>
                </v-dialog>
                <v-dialog v-model="dialogjoin" max-width="500px">
                    <v-card class="pa-2">
                        <v-card-title>Berhasil Bergabung</v-card-title>
                            <v-card-text class="text-justify px-6">Terima kasih kamu telah bersedia bergabung pada kegiatan ini! Selanjutnya silahkan masuk ke dalam grup yang telah disediakan untuk mendapat pengarahan selanjutnya.</v-card-text>
                            <div class="pa-3">
                                <v-btn color="primary" width="100%" class="pa-2 mb-3" @click="dialogjoin=false">Masuk Grup WhatsApp</v-btn>
                            </div>
                    </v-card>
                </v-dialog>
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
            </v-row>
        </v-toolbar>
    </div>
</template>
<script>
    export default {
        methods:{
            copy() {
                alert('Nomor Rekening Berhasil Tersalin')
            }
    },

    data () {
        return {
            dialog: false,
            dialog2: false,
            dialogjoin: false,
            dialoginputnominal: false,
            dialogrekeninglist: false,
            dialogdetaildonasi: false,
            jobs: [
                { text: 'CUSTOMER RELATIONSHIP' },
                { text: 'GRAPHICS DESIGNER' },
                { text: 'PERLENGKAPAN' },
                { text: 'LIAISON OFFICER' },
                { text: 'SPONSORSHIP' },
            ],
        }
    },
    }
</script>
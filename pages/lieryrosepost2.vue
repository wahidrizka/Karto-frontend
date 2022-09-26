<template>
    <div>
        <v-toolbar short>
            <n-link to="/exploregs" class="text-decoration-none">
                <v-btn icon>
                    <v-icon>mdi-arrow-left</v-icon>
                </v-btn>
            </n-link>
            <v-toolbar-title>
                <h5>Postingan Lily Erosu</h5>
            </v-toolbar-title>
        </v-toolbar>
        <div class="ml-3 mt-5 d-flex">
            <v-avatar size="62">
                <v-img src="https://s3-alpha-sig.figma.com/img/b28b/bb19/659ec7f893661f98c6bb623a0cfbc2fb?Expires=1598227200&Signature=M7P1C~yimLtObGktG9KK~fPGme6L~gcfg0w1e69y4SEUOEbPCIUUTDuzEE6JTDuFIutHeuWFq4TPM-5M8Kl6hQ~ZvLu5fOyIEgSjK50texIRjBLznFBxiKRfmSdkL1PaGHuNowIo9Cuux3fGUE-5jJHm6jwUPqFgXNvloZDSZEDSjIGPkD4Zg65L2JriVsF3gTdsuoAEQdHjwR4enPGyMXMgreUOXLTRx-ZFram90vS1DQvWmqeejPN7gPEuziX16BrVYjYFR44uKguJjyuFVTmXNm3i2MiFNz9b3-Hz5OdYObIEyt~mY6AnBith9XOg1S6lLSRmVTT01BgHPq8ZMA__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA"></v-img>
            </v-avatar>
            <div class="flex-column ml-3">
                <h4 class="mb-1">Lily Erosu<v-icon color="blue accent" small class="mb-1 ml-2">mdi-check-circle</v-icon></h4>
                <p class="font-weight-light">liery_rose</p>
            </div>
        </div>
        <v-carousel height="250"
            :show-arrows="false"
            delimiter-icon=mdi-circle-medium>
            <v-carousel-item
                src="https://s3-alpha-sig.figma.com/img/8bac/cbd7/a9f81ac00c4c801619372fc2c501ac10?Expires=1598227200&Signature=BT-bWeF51OAsJRq8KrMiitref6KjHX3MnboTzJBeEa9QIfknck83kQigz1U4nfKfRDrUWcO3eLABPSZ34gvHpVQiXaZ5z6AJW-BQUJRlmgmGU4L98wLeryzvJVGTQNVxFAo30kKN~WSKXS1L4ovfSfFPUqH0nArNGbMEPjEEwRMMnC0~8L0oyFIATA1kkwzUUBfB7TWifPNHeZUQ1H73AN3oJNqVimpU8AVaSqhsPNH3cKR8Z3SSe1uJacyF8YLRiBhWH5GLqoLNF5gmT8AmRQ5HXXLwCJeBc0oGB7LyIqq42CCCKf0S0rYWjFzwYXkpFy9Xmmge44lZN8GoJSVbCg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
            </v-carousel-item>
            <v-carousel-item
                src="https://s3-alpha-sig.figma.com/img/8bac/cbd7/a9f81ac00c4c801619372fc2c501ac10?Expires=1598227200&Signature=BT-bWeF51OAsJRq8KrMiitref6KjHX3MnboTzJBeEa9QIfknck83kQigz1U4nfKfRDrUWcO3eLABPSZ34gvHpVQiXaZ5z6AJW-BQUJRlmgmGU4L98wLeryzvJVGTQNVxFAo30kKN~WSKXS1L4ovfSfFPUqH0nArNGbMEPjEEwRMMnC0~8L0oyFIATA1kkwzUUBfB7TWifPNHeZUQ1H73AN3oJNqVimpU8AVaSqhsPNH3cKR8Z3SSe1uJacyF8YLRiBhWH5GLqoLNF5gmT8AmRQ5HXXLwCJeBc0oGB7LyIqq42CCCKf0S0rYWjFzwYXkpFy9Xmmge44lZN8GoJSVbCg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
            </v-carousel-item>
            <v-carousel-item
                src="https://s3-alpha-sig.figma.com/img/8bac/cbd7/a9f81ac00c4c801619372fc2c501ac10?Expires=1598227200&Signature=BT-bWeF51OAsJRq8KrMiitref6KjHX3MnboTzJBeEa9QIfknck83kQigz1U4nfKfRDrUWcO3eLABPSZ34gvHpVQiXaZ5z6AJW-BQUJRlmgmGU4L98wLeryzvJVGTQNVxFAo30kKN~WSKXS1L4ovfSfFPUqH0nArNGbMEPjEEwRMMnC0~8L0oyFIATA1kkwzUUBfB7TWifPNHeZUQ1H73AN3oJNqVimpU8AVaSqhsPNH3cKR8Z3SSe1uJacyF8YLRiBhWH5GLqoLNF5gmT8AmRQ5HXXLwCJeBc0oGB7LyIqq42CCCKf0S0rYWjFzwYXkpFy9Xmmge44lZN8GoJSVbCg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
            </v-carousel-item>
        </v-carousel>
        <div class="d-flex mt-1 justify-space-around">
            <div class="d-flex">
                <v-btn disabled icon color="blue accent">
                    <v-icon>mdi-progress-clock</v-icon>
                </v-btn>
                <p class="caption font-weight-bold mt-2">16 Hari Lagi</p>
            </div>
            <div class="d-flex">
                <v-btn disabled icon color="blue accent">
                    <v-icon>mdi-thumb-up-outline</v-icon>
                </v-btn>
                <p class="caption font-weight-bold mt-2">1,1 Ribu Mendukung</p>
            </div>
            <div>
                <v-btn icon color="blue accent">
                    <v-icon>mdi-share</v-icon>
                </v-btn>
            </div>
        </div>
        <h3>Gerakan Mahasiswa Anti-Hoax</h3>
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
            <v-avatar color="blue accent" size="33">
                <span class="caption white--text">25+</span>
            </v-avatar>
        </div>

        <h4 class="mt-5">Donasi Terkumpul</h4>
        <v-progress-linear rounded color="blue accent" height="10" value="83"></v-progress-linear>
        <p class="caption font-weight-bold">Uang : Rp 8.337.000 / Rp 10.000.000</p>
        <h4 class="mt-4">Deskripsi :</h4>
        <p class="text-justify">Mahasiswa harus pintar dalam menyampaikan pesan dan menerimanya. Terlebih, dierami digital ini banyak hoax menyerang sosial media. Maka dari itu, mahasiswa harus pintar memilah informasi.</p>
        <h4>Detail Kegiatan</h4>
        <div>
            <p><v-icon class="mr-2">mdi-calendar</v-icon>10-31 Agustus</p>
            <p><v-icon class="mr-2">mdi-map-marker</v-icon>Condong Catur</p>
            <p><v-icon class="mr-2">mdi-briefcase-variant-outline</v-icon>5 Peran Tersedia</p>
            <p><v-icon class="mr-2">mdi-face-outline</v-icon>13 Teman Kamu Juga Berpartisipasi</p>
        </div>
        <h4>Titik Kumpul / Lokasi Gerakan</h4>
        <div class="mx-auto text-center mb-3">
            <iframe
                width="300"
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3953.3118870080016!2d110.3936679143762!3d-7.756708579067883!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e7a59a6c5c395b5%3A0x68950f60e5778641!2sCondong%20Catur%20Bus%20Terminal!5e0!3m2!1sen!2sid!4v1597894481108!5m2!1sen!2sid" 
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
                <v-btn color="blue accent" class="ma-2" @click="dialog = true">
                    Gabung Relawan
                </v-btn>
                <v-btn color="blue accent" class="ma-2" @click="dialoginputnominal = true">
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
                <v-dialog v-model="dialogjoin" max-width="500px">
                    <v-card class="pa-2">
                        <v-card-title>Berhasil Bergabung</v-card-title>
                            <v-card-text class="text-justify px-6">Terima kasih kamu telah bersedia bergabung pada kegiatan ini! Selanjutnya silahkan masuk ke dalam grup yang telah disediakan untuk mendapat pengarahan selanjutnya.</v-card-text>
                            <div class="pa-3">
                                <v-btn color="blue accent" width="100%" class="pa-2 mb-3" @click="dialogjoin=false">Masuk Grup WhatsApp</v-btn>
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
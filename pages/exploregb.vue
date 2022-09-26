<template>
    <v-app>
            <div>
                <v-text-field solo dense label="Cari campaign..." prepend-inner-icon="mdi-magnify">
                </v-text-field>
                <div class="text-center d-flex justify-center">
                    <div class="mx-auto">
                        <v-btn small outlined fab elevation="1" color="primary">
                            <v-icon>mdi-alert-outline</v-icon>
                        </v-btn>
                        <p class="font-weight-bold caption">Bencana<br>Alam</p>
                    </div>
                    <div class="mx-auto">
                        <v-btn small outlined fab elevation="1" color="primary">
                            <v-icon>mdi-school-outline</v-icon>
                        </v-btn>
                        <p class="font-weight-bold caption">Beasiswa<br>Pendidikan</p>
                    </div>
                    <div class="mx-auto">
                        <v-btn small outlined fab elevation="1" color="primary">
                            <v-icon>mdi-hospital-box-outline</v-icon>
                        </v-btn>
                        <p class="font-weight-bold caption">Bantuan<br>Medis</p>
                    </div>
                    <div class="mx-auto">
                        <v-btn small outlined fab elevation="1" color="primary">
                            <v-icon>mdi-package-variant</v-icon>
                        </v-btn>
                        <p class="font-weight-bold caption">Produk<br>Inovasi</p>
                    </div>
                    <div class="mx-auto">
                        <n-link to="/kategori" class="text-decoration-none">
                        <v-btn small outlined fab elevation="1" color="primary">
                            <v-icon>mdi-view-headline</v-icon>
                        </v-btn>
                        <p class="font-weight-bold caption">Lainnya</p>
                        </n-link>
                    </div>
                </div>
                <v-divider></v-divider>
                <div class="my-7">
                    <div class=" mb-1 d-flex justify-space-between">
                        <div>
                        <v-avatar size="40">
                            <img src="https://marucco-lino.com/wp-content/uploads/2019/06/%E6%A3%AE%E4%B8%83%E8%8F%9C.jpg">
                        </v-avatar>
                        <span class="mx-3 captio font-weight-bold">MoriNana
                            <v-icon x-small color="blue" class="mx-1">mdi-check-circle</v-icon>
                        </span>
                        </div>
                        <div class="pt-2">
                            <span class="text-caption"><v-icon class="mr-1 mb-1">mdi-progress-clock</v-icon>Berakhir 31 Agustus</span>
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
                    <div class="d-flex mt-1 justify-space-between">
                        <div class="d-flex">
                            <v-btn icon color="primary">
                                <v-icon>mdi-thumb-up-outline</v-icon>
                            </v-btn>
                            <p class="text-right ml-1 mt-2 caption font-weight-bold">1,1 Ribu Mendukung</p>
                        </div>
                        <v-btn icon color="primary">
                            <v-icon>mdi-share</v-icon>
                        </v-btn>                       
                    </div>
                    <div>
                        <n-link to="/morinanapost1" class="text-decoration-none">
                            <h3>Kaori Menderita Kanker Stadium 3</h3>
                        </n-link>
                        <v-clamp autoresize :max-lines="3" :expanded="expanded">
                            {{text}}
                                <template v-slot:after="{ clamped, toggle }">
                                    <v-btn text small @click="toggle()">
                                        <span v-if="clamped">Selengkapnya</span> 
                                        <span v-else>Lebih sedikit</span> 
                                    </v-btn>
                                </template>
                        </v-clamp>
                    </div>
                </div>
                <div class="my-7">
                    <div class="mb-1 d-flex justify-space-between">
                        <div>
                        <v-avatar size="40">
                            <img src="https://s3-alpha-sig.figma.com/img/b28b/bb19/659ec7f893661f98c6bb623a0cfbc2fb?Expires=1598227200&Signature=M7P1C~yimLtObGktG9KK~fPGme6L~gcfg0w1e69y4SEUOEbPCIUUTDuzEE6JTDuFIutHeuWFq4TPM-5M8Kl6hQ~ZvLu5fOyIEgSjK50texIRjBLznFBxiKRfmSdkL1PaGHuNowIo9Cuux3fGUE-5jJHm6jwUPqFgXNvloZDSZEDSjIGPkD4Zg65L2JriVsF3gTdsuoAEQdHjwR4enPGyMXMgreUOXLTRx-ZFram90vS1DQvWmqeejPN7gPEuziX16BrVYjYFR44uKguJjyuFVTmXNm3i2MiFNz9b3-Hz5OdYObIEyt~mY6AnBith9XOg1S6lLSRmVTT01BgHPq8ZMA__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
                        </v-avatar>
                        <span class="mx-3 captio font-weight-bold">Lily Erosu
                            <v-icon x-small color="blue" class="mx-1">mdi-check-circle</v-icon>
                        </span>
                        </div>
                        <div>
                        <div class="pt-2">
                            <span class="text-caption"><v-icon class="mr-1 mb-1">mdi-progress-clock</v-icon>Berakhir 31 Agustus</span>
                        </div>
                        </div>
                    </div>
                    <v-carousel height="250"
                        :show-arrows="false"
                        delimiter-icon=mdi-circle-medium>
                        <v-carousel-item
                            src="https://s3-alpha-sig.figma.com/img/1776/d1e6/f462175ee5617002577a57f7c85fa55d?Expires=1598227200&Signature=MzYUqCkDeDnVmUTtbQxE~ajG0oF3XcDC9TqGhQM9fWzL2xtVljpP5kzVc6fS80wO~rdehl8q0cbAYpc-5JfATQN5G11pDxxeZQUUAlzog3HL4v6g~CW-e76z-iZ00pQ5mqjolEll5kQ3A7cWBF0Aah8GKY66tRsuBJecw6dx1rUrx-zjiN04q6olIINMn7YxEi3zYREeblPKge~8VkEiHu~DvY0t7yDqMnGRpK4O1DC5UrwoJ--JRcf3nhn0jq1BZAAwMdaBl8wkx3aviewMfQZ1~p2aTIp5N5aS8~9LZNn-N1gsBBR5QLiCRXjd~msMFYwqzaJAwCYTGYvdUZWXLw__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
                        </v-carousel-item>
                        <v-carousel-item
                            src="https://s3-alpha-sig.figma.com/img/1776/d1e6/f462175ee5617002577a57f7c85fa55d?Expires=1598227200&Signature=MzYUqCkDeDnVmUTtbQxE~ajG0oF3XcDC9TqGhQM9fWzL2xtVljpP5kzVc6fS80wO~rdehl8q0cbAYpc-5JfATQN5G11pDxxeZQUUAlzog3HL4v6g~CW-e76z-iZ00pQ5mqjolEll5kQ3A7cWBF0Aah8GKY66tRsuBJecw6dx1rUrx-zjiN04q6olIINMn7YxEi3zYREeblPKge~8VkEiHu~DvY0t7yDqMnGRpK4O1DC5UrwoJ--JRcf3nhn0jq1BZAAwMdaBl8wkx3aviewMfQZ1~p2aTIp5N5aS8~9LZNn-N1gsBBR5QLiCRXjd~msMFYwqzaJAwCYTGYvdUZWXLw__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
                        </v-carousel-item>
                        <v-carousel-item
                            src="https://s3-alpha-sig.figma.com/img/1776/d1e6/f462175ee5617002577a57f7c85fa55d?Expires=1598227200&Signature=MzYUqCkDeDnVmUTtbQxE~ajG0oF3XcDC9TqGhQM9fWzL2xtVljpP5kzVc6fS80wO~rdehl8q0cbAYpc-5JfATQN5G11pDxxeZQUUAlzog3HL4v6g~CW-e76z-iZ00pQ5mqjolEll5kQ3A7cWBF0Aah8GKY66tRsuBJecw6dx1rUrx-zjiN04q6olIINMn7YxEi3zYREeblPKge~8VkEiHu~DvY0t7yDqMnGRpK4O1DC5UrwoJ--JRcf3nhn0jq1BZAAwMdaBl8wkx3aviewMfQZ1~p2aTIp5N5aS8~9LZNn-N1gsBBR5QLiCRXjd~msMFYwqzaJAwCYTGYvdUZWXLw__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
                        </v-carousel-item>
                        <v-carousel-item
                            src="https://s3-alpha-sig.figma.com/img/1776/d1e6/f462175ee5617002577a57f7c85fa55d?Expires=1598227200&Signature=MzYUqCkDeDnVmUTtbQxE~ajG0oF3XcDC9TqGhQM9fWzL2xtVljpP5kzVc6fS80wO~rdehl8q0cbAYpc-5JfATQN5G11pDxxeZQUUAlzog3HL4v6g~CW-e76z-iZ00pQ5mqjolEll5kQ3A7cWBF0Aah8GKY66tRsuBJecw6dx1rUrx-zjiN04q6olIINMn7YxEi3zYREeblPKge~8VkEiHu~DvY0t7yDqMnGRpK4O1DC5UrwoJ--JRcf3nhn0jq1BZAAwMdaBl8wkx3aviewMfQZ1~p2aTIp5N5aS8~9LZNn-N1gsBBR5QLiCRXjd~msMFYwqzaJAwCYTGYvdUZWXLw__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
                        </v-carousel-item>
                        <v-carousel-item
                            src="https://s3-alpha-sig.figma.com/img/1776/d1e6/f462175ee5617002577a57f7c85fa55d?Expires=1598227200&Signature=MzYUqCkDeDnVmUTtbQxE~ajG0oF3XcDC9TqGhQM9fWzL2xtVljpP5kzVc6fS80wO~rdehl8q0cbAYpc-5JfATQN5G11pDxxeZQUUAlzog3HL4v6g~CW-e76z-iZ00pQ5mqjolEll5kQ3A7cWBF0Aah8GKY66tRsuBJecw6dx1rUrx-zjiN04q6olIINMn7YxEi3zYREeblPKge~8VkEiHu~DvY0t7yDqMnGRpK4O1DC5UrwoJ--JRcf3nhn0jq1BZAAwMdaBl8wkx3aviewMfQZ1~p2aTIp5N5aS8~9LZNn-N1gsBBR5QLiCRXjd~msMFYwqzaJAwCYTGYvdUZWXLw__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
                        </v-carousel-item>
                    </v-carousel>
                    <div class="d-flex mt-1 justify-space-between">
                        <div class="d-flex">
                            <v-btn icon color="primary">
                                <v-icon>mdi-thumb-up-outline</v-icon>
                            </v-btn>
                            <p class="text-right ml-1 mt-2 caption font-weight-bold">1,1 Ribu Mendukung</p>
                        </div>
                        <v-btn icon color="primary">
                            <v-icon>mdi-share</v-icon>
                        </v-btn>                       
                    </div>
                    <div>
                        <n-link to="/lieryrosepost1" class="text-decoration-none">
                            <h3>BisaMakanDaging - Berbagi Daging Untuk Dhuafa</h3>
                        </n-link>
                        <v-clamp autoresize :max-lines="3" :expanded="expanded">
                            {{ text1 }}
                                <template v-slot:after="{ clamped, toggle }">
                                    <v-btn text small @click="toggle()">
                                        <span v-if="clamped">Selengkapnya</span> 
                                        <span v-else>Lebih sedikit</span> 
                                    </v-btn>
                                </template>
                        </v-clamp>
                    </div>
                </div>
            </div>
    </v-app>
</template>
<script>
import VClamp from 'vue-clamp'
export default {
    components: {
        VClamp
    },
    data () {
        return {
            expanded: false,
            text : 'Penyakit tersebut membuat tubuh Kaori menjadi lemah dan dirinya kesulitan untuk berdiri hingga akhirnya ia harus dirawat di rumah sakit selama beberapa hari. Penyakit yang dialami oleh Kaori telah dijelaskan langsung oleh dokter, bahwa Kaori mengidap penyakit kanker yang mematikan, serta penyakit sumsum tulang.',
            text1 : 'Dalam kondisi pandemi seperti ini, saya melihat kaum dhuafa terdampak begitu besar. banyak anak-anak hingga para lansia dhuafa yang tak bisa memenuhi kebutuhan gizi mereka karena sulitnya kondisi perekonomian. "Bisa makan sama garam saja sudah Alhamdulilah, bu..." Begitu ucap mereka..'
        }
    }
}
</script>
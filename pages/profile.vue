<template>
    <v-app>
            <div class="d-flex mt-3">
                <v-avatar size="100">
                        <img src="https://marucco-lino.com/wp-content/uploads/2019/06/%E6%A3%AE%E4%B8%83%E8%8F%9C.jpg">
                </v-avatar>
                <v-row no-gutters class="justify-space-around text-center">
                    <v-col cols=4 xs="4" md="3">
                        <n-link to="/pengikut" class="text-decoration-none">
                        <div>
                            <h4>999</h4>
                            <p>Pengikut</p>
                        </div>
                        </n-link>
                    </v-col>
                    <v-col cols=4 xs="4" md="3">
                        <n-link to="/mengikuti" class="text-decoration-none">
                        <div>
                            <h4>39</h4>
                            <p>Mengikuti</p>
                        </div>
                        </n-link>
                    </v-col>
                    <v-col cols="12" sm="6" md="4" lg="3">
                        <n-link to="/editprofile" class="text-decoration-none">
                            <v-btn outlined color="primary">Edit Profil</v-btn>
                        </n-link>
                    </v-col>
                </v-row>              
            </div>
            <div class="mt-2">
                <v-col>
                    <h3>MoriNana <v-icon color="primary" small class="mb-1">mdi-check-circle</v-icon></h3>
                    <p class="font-weight-light">nanamori</p>
                    <h4 class="font-weight-regular">Sesungguhnya Harta hanyalah titipan dari Allah SWT.</h4>
                </v-col>
            </div>
            <div class="d-flex justify-space-around">
                <p class="caption">
                    <v-icon class="mb-1" small>mdi-map-marker</v-icon>   
                    Batikan, Juwiring
                </p>
                <n-link to="#" class="text-decoration-none">
                    <p class="caption">
                        <v-icon class="mb-1" small>mdi-link-variant</v-icon>   
                        morina.moe
                    </p>
                </n-link>
            </div>
        <div>
            <v-tabs fixed-tabs icons-and-text>
                <v-tab key="donasi">
                    <p class="caption font-weight-bold">Donasi</p>
                    <v-icon>mdi-hand-heart-outline</v-icon>
                </v-tab>
                <v-tab key="penggalangan">
                    <p class="caption font-weight-bold">Penggalangan</p>
                    <v-icon>mdi-spa-outline</v-icon>
                </v-tab>
                <v-tab key="gerakan">
                    <p class="caption font-weight-bold">Gerakan</p>
                    <v-icon>mdi-account-group-outline</v-icon>
                </v-tab>
                <v-tab-item key="donasi">
                    <div class="mt-2 d-flex" style="overflow-x:auto">
                        <v-btn small color="primary" class="ma-4" rounded elevation="3">2020</v-btn>
                        <v-btn small class="ma-4" rounded elevation="3">2019</v-btn>
                        <v-btn small class="ma-4" rounded elevation="3">2018</v-btn>
                        <v-btn small class="ma-4" rounded elevation="3">2017</v-btn>
                        <v-btn small class="ma-4" rounded elevation="3">2016</v-btn>
                    </div>
                    <div>
                        <p>Agustus 2020</p>
                        <v-timeline align-top dense>
                            <v-timeline-item icon="mdi-cash">
                                <p>Donasi Rp. 100.000</p>
                                <v-card shaped class="mt-5">
                                    <v-img src="https://i1.wp.com/newsrush.in/wp-content/uploads/2020/07/doctors-day-2020-a-medic-shares-how-hard-lockdown-has-been-for-cancer-patients.jpg?w=1020&ssl=1"></v-img>
                                    <v-card-text>
                                        <h4>Kaori Menderita Kanker Stadium 3</h4>
                                    </v-card-text>
                                </v-card>
                            </v-timeline-item>
                        </v-timeline>
                        <p>Juli 2020</p>
                        <v-timeline align-top dense>
                            <v-timeline-item icon="mdi-food-steak">
                                <p>Donasi Daging 1kg</p>
                                <v-card shaped class="mt-5">
                                    <v-img src="https://s3-alpha-sig.figma.com/img/1776/d1e6/f462175ee5617002577a57f7c85fa55d?Expires=1598227200&Signature=MzYUqCkDeDnVmUTtbQxE~ajG0oF3XcDC9TqGhQM9fWzL2xtVljpP5kzVc6fS80wO~rdehl8q0cbAYpc-5JfATQN5G11pDxxeZQUUAlzog3HL4v6g~CW-e76z-iZ00pQ5mqjolEll5kQ3A7cWBF0Aah8GKY66tRsuBJecw6dx1rUrx-zjiN04q6olIINMn7YxEi3zYREeblPKge~8VkEiHu~DvY0t7yDqMnGRpK4O1DC5UrwoJ--JRcf3nhn0jq1BZAAwMdaBl8wkx3aviewMfQZ1~p2aTIp5N5aS8~9LZNn-N1gsBBR5QLiCRXjd~msMFYwqzaJAwCYTGYvdUZWXLw__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA"></v-img>
                                    <v-card-text>
                                        <h4>BisaMakanDaging - Berbagi Daging Untuk Dhuafa</h4>
                                    </v-card-text>
                                </v-card>
                            </v-timeline-item>
                        </v-timeline>
                    </div>
                </v-tab-item>
                <v-tab-item key="penggalangan">
                    <div class="my-7">
                    <div class="ma-2 d-flex justify-space-between">
                        <div>
                        <v-avatar size="40">
                            <img src="https://marucco-lino.com/wp-content/uploads/2019/06/%E6%A3%AE%E4%B8%83%E8%8F%9C.jpg">
                        </v-avatar>
                        <span class="mx-3 captio font-weight-bold">MoriNana
                            <v-icon x-small color="blue" class="mx-1">mdi-check-circle</v-icon>
                        </span>
                        </div>
                        <div>
                            <n-link to="/morinanapost1" class="text-decoration-none">
                            <v-btn outlined class="mt-1 ml-1" small color="primary">
                                Lihat Postingan
                            </v-btn>
                        </n-link>
                        </div>
                    </div>
                    <v-carousel height="250"
                        :show-arrows="false"
                        delimiter-icon="mdi-circle-medium">
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
                            <v-btn icon color="primary">
                                <v-icon>mdi-share-outline</v-icon>
                            </v-btn>
                        </div>
                        <div class="mt-2">
                            <p class="text-right ml-1 caption font-weight-bold">1,1 Ribu Mendukung</p>
                        </div>
                    </div>
                    <div>
                        <h3>Kaori Menderita Kanker Stadium 3</h3>
                        <v-clamp autoresize :max-lines="1" :expanded="expanded">
                            {{ text }}
                                <template v-slot:after="{ clamped, toggle }">
                                    <v-btn text small @click="toggle()">
                                        <span v-if="clamped">Selengkapnya</span> 
                                        <span v-else>Lebih sedikit</span> 
                                    </v-btn>
                                </template>
                        </v-clamp>
                    </div>
                </div>
                </v-tab-item>
                <v-tab-item key="gerakan">
                    <v-container class="text-center my-16">
                        Belum Ada Gerakan Sosial Dibuat
                    </v-container>
                </v-tab-item>
            </v-tabs>
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
            text : 'Penyakit tersebut membuat tubuh Kaori menjadi lemah dan dirinya kesulitan untuk berdiri hingga akhirnya ia harus dirawat di rumah sakit selama beberapa hari. Penyakit yang dialami oleh Kaori telah dijelaskan langsung oleh dokter, bahwa Kaori mengidap penyakit kanker yang mematikan, serta penyakit sumsum tulang.'
        }
    }
}
</script>

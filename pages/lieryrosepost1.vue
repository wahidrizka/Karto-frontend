<template>
    <div>
        <v-toolbar short>
            <n-link to="/exploregb" class="text-decoration-none">
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
                <h4 class="mb-1">Lily Erosu<v-icon small class="mb-1 ml-2">mdi-check-circle</v-icon></h4>
                <p class="font-weight-light">liery_rose</p>
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
        <div class="d-flex mt-1 justify-space-around">
            <div class="d-flex">
                <v-btn disabled icon color="blue accent">
                    <v-icon>mdi-progress-clock</v-icon>
                </v-btn>
                <p class="caption font-weight-bold mt-2">13 Hari Lagi</p>
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
        <h3>BisaMakanDaging - Berbagi Daging Untuk Dhuafa</h3>
        <h4 class="mt-2 font-weight-bold">Bantuan Dibutuhkan</h4>
        <v-card class="my-2">
            <div class="d-flex justify-space-between pa-2 pt-4">
                <p><v-icon color="blue accent">mdi-food-steak</v-icon> Daging</p>
                <n-link to="kontak&lokasi" class="text-decoration-none">
                    <v-btn color="blue accent" outlined small>Kontak Penggalang</v-btn>
                </n-link>
            </div>
        </v-card>
        <h4 class="my-3">Donasi Terkumpul</h4>
        <v-progress-linear rounded color="blue accent" height="10" value="83"></v-progress-linear>
        <p class="caption font-weight-bold">Uang : Rp 8.337.000 / Rp 10.000.000</p>
        <v-progress-linear color="blue accent" height="10" value="31" rounded></v-progress-linear>
        <p class="caption font-weight-bold">Daging : 31 Kg / 100 Kg</p>
        <h4>Cerita Penggalang :</h4>
        <p class="text-justify">Dalam kondisi pandemi seperti ini, saya melihat kaum dhuafa terdampak begitu besar.</p>
        <p class="text-justify">Banyak anak-anak hingga para lansia dhuafa yang tak bisa memenuhi kebutuhan gizi mereka karena sulitnya kondisi perekonomian.</p>
        <p class="text-justify">"Bisa makan sama garam saja sudah Alhamdulilah, bu...", Begitu ucap mereka.</p>
        <div class="mx-auto text-center mb-3">
            <iframe
                width="300"
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3953.3135475577956!2d110.40563394906836!3d-7.75653189438218!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e7a599e9f3478d7%3A0xf24e64d67f7cf706!2sMasjid%20Muhajirin!5e0!3m2!1sen!2sid!4v1597895987474!5m2!1sen!2sid" 
                frameborder="0" 
                style="border:0;" 
                allowfullscreen="" 
                aria-hidden="false">
            </iframe>
        </div>
        <div>
            <v-badge text inline content="0">
                <h4>Kabar Terbaru</h4>
            </v-badge>
            <v-card height="100" class="text-center mx-auto">
                <p>Belum ada kabar terbaru</p>
            </v-card>
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
<template>
  <v-app>
      <div class="text-center pb-4 d-flex justify-center">
        <v-text-field solo dense label="Cari campaign..." prepend-inner-icon="mdi-magnify">
        </v-text-field>
      </div>
      <div class="pb-4">
        <v-card flat color="grey lighten-2" class="text-center d-flex justify-center">
          <div class="mx-auto my-4">
            <n-link to="/buatgb" class="text-decoration-none">
              <v-icon color="primary" class="mb-2" large>mdi-spa-outline</v-icon>
            </n-link>
            <h6>Buat <br>Galang Bantuan</h6>
          </div>
          <div class="mx-auto my-4">
            <n-link to="/exploregb" class="text-decoration-none">
              <v-icon color="primary" class="mb-2" large>mdi-hand-heart-outline</v-icon>
            </n-link>
            <h6>Explore <br>Galang Bantuan</h6>
          </div>
          <div class="mx-auto my-4">
            <n-link to="/buatgs" class="text-decoration-none">
              <v-icon color="primary" class="mb-2" large>mdi-account-multiple-plus-outline</v-icon>
            </n-link>
            <h6>Buat <br>Gerakan Sosial</h6>
          </div>
          <div class="mx-auto my-4">
            <n-link to="/exploregs" class="text-decoration-none">
              <v-icon color="primary" class="mb-2" large>mdi-account-group-outline</v-icon>
            </n-link>
            <h6>Explore <br>Gerakan Sosial</h6>
          </div>
        </v-card>
      </div>
      <div class="pt-5 pb-4">
        <h2>Perlu Bantuan Segera</h2>
        <div style="overflow-x:auto;" class="my-3 d-flex">
          <CampaignCard v-for="(campaign, index) in campaigns"
            :key="index"
            :link="campaign.link"
            :img="campaign.img"
            :title="campaign.title"
            :location="campaign.location"
          />
        </div>
      </div>
      <div class="pt-5 pb-4">
        <h2>Gerakan Sosial Pilihan</h2>
        <div style="overflow-x:auto;" class="my-3 d-flex">
          <n-link to="/lieryrosepost2" class="text-decoration-none">
            <v-card class="ma-3">
            <v-img
              src="https://s3-alpha-sig.figma.com/img/8bac/cbd7/a9f81ac00c4c801619372fc2c501ac10?Expires=1598227200&Signature=BT-bWeF51OAsJRq8KrMiitref6KjHX3MnboTzJBeEa9QIfknck83kQigz1U4nfKfRDrUWcO3eLABPSZ34gvHpVQiXaZ5z6AJW-BQUJRlmgmGU4L98wLeryzvJVGTQNVxFAo30kKN~WSKXS1L4ovfSfFPUqH0nArNGbMEPjEEwRMMnC0~8L0oyFIATA1kkwzUUBfB7TWifPNHeZUQ1H73AN3oJNqVimpU8AVaSqhsPNH3cKR8Z3SSe1uJacyF8YLRiBhWH5GLqoLNF5gmT8AmRQ5HXXLwCJeBc0oGB7LyIqq42CCCKf0S0rYWjFzwYXkpFy9Xmmge44lZN8GoJSVbCg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA"
              width="250px" max-height="133">
            </v-img>
            <h3 class="ml-1">Gerakan Mahasiswa <br>Anti-Hoax</h3>
            <div class="flex-row subtitle-1 text-caption">
              <v-icon class="ma-1">mdi-calendar</v-icon>10-31 Agustus 2020<br>
              <v-icon class="ma-1">mdi-map-marker</v-icon>Condong Catur<br>
              <v-icon class="ma-1">mdi-briefcase-variant-outline</v-icon>27 Kategori Peran
            </div>
            <div class="ma-2">
              <v-progress-linear color="blue" height="7" rounded value="80"></v-progress-linear>
              <p class="text-caption">Relawan: 32 dari 140</p>
              <v-progress-linear color="blue" height="7" rounded value="83.77"></v-progress-linear>
              <p class="text-caption">Donasi: Rp8.337.000 / Rp10.000.000 </p>
            </div>
          </v-card>
          </n-link>
          <n-link to="/lieryrosepost1" class="text-decoration-none">
            <v-card class="ma-3">
            <v-img
              src="https://s3-alpha-sig.figma.com/img/11ff/b873/e740a936916f49650ddbac60b037964f?Expires=1598227200&Signature=CfidJWioip8KXdWxxSHuuSnNzLLS~if8NT5hYiyxPAr-xHsno~jPQbTJg8lMuvyTt1jP~~9ffq97JVoALCSyNl3pb8tDPzKms~3v4KDIZrpwpwAhlMa72np2mSW746Bl2uPdiJRTJN~rmoX3Stc8WlFOrC9Zht5hYzE37UThU~B1BPPWvDJWnvQJRoGKXvvWU9m8tlZ7DrYle71rs5g2BqdqH~9BTwRFXIfupFKRbndVMm67Tq9y4jIodG3XKdEWtl8NGiX0qdM87wYz7BwGwblz9OYcc4SKFyd1p1FC8pkfdqvncuV4PTtZ1ti46zpnEKhOLAc76y1EkYWYeNQmww__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA"
              width="250px" max-height="133">
            </v-img>
            <h3 class="ml-1">Aksi Tebar Daging Qurban <br>Melintasi Batas</h3>
            <div class="flex-row subtitle-1 text-caption">
              <v-icon class="ma-1">mdi-calendar</v-icon>10-31 Agustus 2020<br>
              <v-icon class="ma-1">mdi-map-marker</v-icon>Condong Catur<br>
              <v-icon class="ma-1">mdi-briefcase-variant-outline</v-icon>27 Kategori Peran
            </div>
            <div class="ma-2">
              <v-progress-linear color="blue" height="7" rounded value="80"></v-progress-linear>
              <p class="text-caption">Uang: Rp8.337.000 / Rp10.000.000</p>
              <v-progress-linear color="blue" height="7" rounded value="83.77"></v-progress-linear>
              <p class="text-caption">Daging: 31kg / 100kg </p>
            </div>
          </v-card>
          </n-link>
        </div>
      </div>
  </v-app>
</template>

<script>
import CampaignCard from '~/components/CampaignCard'

export default {
  data: () => ({
    campaigns: [
      {
        link: '/morinanapost1',
        img: 'https://i1.wp.com/newsrush.in/wp-content/uploads/2020/07/doctors-day-2020-a-medic-shares-how-hard-lockdown-has-been-for-cancer-patients.jpg?w=1020&ssl=1',
        title: 'Kaori Menderita Kanker Stadium 3',
        location: 'Batikan, Juwiring (13km)'
      },
      {
        link: '/lieryrosepost1',
        img: 'https://s3-alpha-sig.figma.com/img/1776/d1e6/f462175ee5617002577a57f7c85fa55d?Expires=1598227200&Signature=MzYUqCkDeDnVmUTtbQxE~ajG0oF3XcDC9TqGhQM9fWzL2xtVljpP5kzVc6fS80wO~rdehl8q0cbAYpc-5JfATQN5G11pDxxeZQUUAlzog3HL4v6g~CW-e76z-iZ00pQ5mqjolEll5kQ3A7cWBF0Aah8GKY66tRsuBJecw6dx1rUrx-zjiN04q6olIINMn7YxEi3zYREeblPKge~8VkEiHu~DvY0t7yDqMnGRpK4O1DC5UrwoJ--JRcf3nhn0jq1BZAAwMdaBl8wkx3aviewMfQZ1~p2aTIp5N5aS8~9LZNn-N1gsBBR5QLiCRXjd~msMFYwqzaJAwCYTGYvdUZWXLw__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA',
        title: 'BisaMakanDaging - Berbagi Daging Untuk Dhuafa',
        location: 'Condong Catur, Sleman (20km)'
      }
    ]
  }),
  components: {
    CampaignCard
  }
}
</script>
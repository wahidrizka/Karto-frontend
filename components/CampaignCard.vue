<template>
  <n-link :to="link" class="text-decoration-none">
    <v-card class="ma-3" width="250">
      <v-img :src="img" width="250px" max-height="133">
      </v-img>
      <div class="pa-3">
        <h3 class="ml-1">
          <VClamp autoresize :max-lines="2">{{ title }}</VClamp>
        </h3>
        <div class="flex-row subtitle-1 text-caption">
          <v-icon class="ma-1">mdi-map-marker</v-icon>{{ location }}<br>
          <v-icon class="ma-1">mdi-swap-vertical</v-icon>1,1rb mendukung
        </div>
      </div>
    </v-card>
  </n-link>
</template>

<script>
import VClamp from 'vue-clamp'
export default {
  name: 'CampaignCard',
  props: ['img', 'link', 'title', 'location'],
  components: {
    VClamp
  }
}
</script>

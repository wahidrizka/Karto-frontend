<template>
  <v-app>
    <!-- Main Content Wrapper -->
    <v-main>
      <v-container fluid>
        <v-row no-gutters>
          <v-col lg="6" offset-lg="3">
            <nuxt />
          </v-col>
        </v-row>
      </v-container>
    </v-main>

    <!-- Bottom Navigation -->
    <v-bottom-navigation
      v-model="bottomNav"
      app
      grow
      color="blue"
      mandatory
      :input-value="showBottomNav"
    >
      <v-btn v-for="nav in navs" :key="nav.name" :to="nav.to" :value="nav.name" height="100%">
        <span>{{ nav.text }}</span>
        <v-icon>{{ nav.icon }}</v-icon>
      </v-btn>
    </v-bottom-navigation>
  </v-app>
</template>

<script>
export default {
  name: 'Default',
  data () {
    return {
      showBottomNav: true,
      bottomNav: this.$route.name
    }
  },
  computed: {
    navs () {
      const items = [
        { to: '/', name: 'beranda', icon: 'mdi-home', text: 'Beranda', show: true },
        { to: '/listgb', name: 'campaign', icon: 'mdi-hand-heart', text: 'Campaign', show: true },
        { to: '/listgs', name: 'grakan', icon: 'mdi-account-group', text: 'Gerakan', show: true },
        { to: '/profile', name: 'profil', icon: 'mdi-account', text: 'Profil', show: true }
      ]
      return items.filter(item => (item.show === true))
    }
  }
}
</script>

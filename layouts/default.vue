<template>
  <v-app dark>
    <v-app-bar fixed app class="bgs">
      <img class="mx-auto" src="../assets/images/logo.png" width="50" />
      <v-btn class="bgs" elevation="0" to="contract_type">
        <span class="white--text">ປະເພດສັນຍາ</span>
      </v-btn>
      <v-btn class="bgs" elevation="0">
        <span class="white--text">ສະຖານະສັນຍາ</span>
      </v-btn>
      <v-btn class="bgs" elevation="0" to="contract_document">
        <span class="white--text">ເອກະສານສັນຍາ</span>
      </v-btn>
      <v-btn class="bgs" elevation="0">
        <span class="white--text">ເອກະສານສັນຍາຮູບແບບແຈ້ງເຕືອນ</span>
      </v-btn>
      <v-spacer></v-spacer>
      <v-btn class="bgs" elevation="0" rounded>
        <span class="white--text">ອອກຈາກລະບົບ</span>
      </v-btn>
    </v-app-bar>
    <v-main>
      <!-- <v-container> -->
      <div class="px-5">
        <Nuxt />
      </div>
      <!-- </v-container> -->
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
    }
  },
}
</script>
<style lang="scss">
.bgs {
  background: linear-gradient(#3c98ce, #2171a1, #144d70);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
}
</style>

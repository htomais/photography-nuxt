<template>
  <v-app>
    <v-app-bar app flat>
      <Header />
    </v-app-bar>

    <v-content>
      <Hero />
      <Gallery />
      <LatestPost />
    </v-content>

    <v-footer>
      <Footer />
    </v-footer>
  </v-app>
</template>

<script>
import Footer from '../components/Footer.vue'
export default {
  components: { Footer },}
</script>

<style></style>

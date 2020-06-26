<template>
  <section class="hero">
    <v-container>
      <v-row align="center">
        <v-col class="text-left">
          <h1 class="text-xl-h3 text-h4 font-weight-light">Calango WEB</h1>
          <h1 class="text-xl-h1 text-h3 font-weight-regular red--text">Desenvolvedor WEB</h1>
          <v-btn outlined rounded class="mt-4" to="/sobre">Vamos lá <v-icon>mdi-arrow-right</v-icon></v-btn>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style>
.hero {
  background-image: url('~@/static/hero.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  height: 100vh;
}

.hero .row,
.hero .container {
  height: 100%;
}
</style>

<script>
export default {
  components: {},
}
</script>

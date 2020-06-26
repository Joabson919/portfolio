<template>
  <section class="back">
    <v-container>
      <v-row class="text-justify px-6" align="center">
        <v-col>
          <h2 class="font-weight-light">Quem sou</h2>
          <h1>Lorem, ipsum dolor sit.</h1>
          <p class="mt-5">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa
            voluptas quis fugiat vero suscipit natus atque. Sint, libero
            deserunt? Nemo, id! Quidem sed illum eius magnam laudantium ipsum
            officiis minus.
          </p>
          <v-btn outlined rounded>
            Contate-me
          </v-btn>
        </v-col>
        <v-col class="hidden-xs-only">
          <v-img max-width="300" src="cell.png" />
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style>
.back {
  background-image: url("~@/static/back.png");
  background-size: cover;
  background-repeat: no-repeat;
}

.back,
.back .row,
.back .container {
  height: 100%;
}
</style>

<script>
export default {
  components: {},
}
</script>

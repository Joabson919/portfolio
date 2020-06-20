<template>
  <v-row align="center" justify="center">
    <v-col sm="8" md="6">
      <v-card>
        <v-card-title class="headline">
          Início
        </v-card-title>
        <v-card-text>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Commodi,
            minima? Possimus repudiandae molestias, quis facere eaque quibusdam
            officiis natus expedita nam laboriosam quo aut similique accusamus
            reprehenderit a voluptatibus odio.
          </p>
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn color="primary" nuxt to="/inspire">
            Continue
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    VuetifyLogo,
  },
}
</script>

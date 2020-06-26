<template>
  <v-app dark>
    <navegacao />
    <v-main class="pt-0">
      <nuxt />
    </v-main>
    <!-- <v-navigation-drawer
      v-model="rightDrawer"
      :right="right"
      temporary
      fixed
    >
      <v-list>
        <v-list-item @click.native="right = !right">
          <v-list-item-action>
            <v-icon light>
              mdi-repeat
            </v-icon>
          </v-list-item-action>
          <v-list-item-title>Switch drawer (click me)</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer> -->
  </v-app>
</template>

<script>
import navegacao from '~/components/layoutPadrao/navegacao.vue'
export default {
  data() {
    return {
      right: true,
      rightDrawer: false,
    }
  },
  created() {
    let tamanho = this.$vuetify.breakpoint.name
    if (tamanho === 'xs' || tamanho === 'sm') {
      this.drawer = false
    } else {
      this.drawer = true
    }
  },
  components: {
    navegacao,
  },
}
</script>

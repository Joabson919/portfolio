<template>
  <div>
    <v-navigation-drawer v-model="drawer" fixed app>
      <v-list class="text-center">
        <v-list-item class="justify-center">
          <v-list-item-icon>
            <v-img src="logo.png" max-width="100"></v-img>
          </v-list-item-icon>
        </v-list-item>
      </v-list>
      <v-divider />
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <template v-slot:append>
        <v-row class="text-center">
          <v-col>
            <v-btn text icon>
              <v-icon>mdi-instagram</v-icon>
            </v-btn>
          </v-col>
          <v-col>
            <v-btn text icon>
              <v-icon>mdi-linkedin</v-icon>
            </v-btn>
          </v-col>
          <v-col>
            <v-btn text icon>
              <v-icon>mdi-github</v-icon>
            </v-btn>
          </v-col>
        </v-row>
      </template>
    </v-navigation-drawer>
    <v-app-bar clipped-left fixed app color="transparent" flat>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" v-if="!drawer" />
      <!-- <v-toolbar-title v-text="title" /> -->
      <v-spacer />
      <!-- <v-btn
        icon
        @click.stop="rightDrawer = !rightDrawer"
      >
        <v-icon>mdi-menu</v-icon>
      </v-btn> -->
    </v-app-bar>
  </div>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
      items: [
        {
          icon: 'mdi-view-dashboard',
          title: 'Início',
          to: '/',
        },
        {
          icon: 'mdi-information-variant',
          title: 'Sobre',
          to: '/sobre',
        },
        {
          icon: 'mdi-format-list-text',
          title: 'Serviços',
          to: '/servicos',
        },
        {
          icon: 'mdi-view-dashboard-variant-outline',
          title: 'Portfólio',
          to: '/portfolio',
        },
        {
          icon: 'mdi-email-outline',
          title: 'Contate-me',
          to: '/contato',
        },
      ],
      title: 'Portfólio',
    }
  },
}
</script>

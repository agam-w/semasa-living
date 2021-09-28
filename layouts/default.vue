<template>
  <v-app dark>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon color="#27cfb1">{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar :clipped-left="clipped" fixed app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <img
        src="../assets/images/semasa-logo.png"
        height="30"
        width="auto"
        alt=""
      />
      <!-- <v-toolbar-title v-text="title" /> -->
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer dark padless>
      <v-card
        flat
        tile
        class="lighten-1 white--text text-center"
        style="background-color: #27cfb1 !important"
        width="100%"
      >
        <v-card-text>
          <v-btn
            v-for="icon in icons"
            :key="icon.image"
            class="mx-4 white--text"
            icon
          >
            <v-icon size="24px" @click.stop.prevent="openWindow(icon.link)">
              {{ icon.image }}
            </v-icon>
          </v-btn>
        </v-card-text>

        <v-card-text class="white--text pt-0">
          Semasa Living is one of the few mileworks that con expertly perform
          this highly skilled work. We offer strong design capability,
          production capacity and local manufacturing expertise.
        </v-card-text>

        <v-divider></v-divider>

        <v-card-text class="white--text">
          {{ new Date().getFullYear() }} — <strong>Semasa Living</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-home',
          title: 'Home',
          to: '/',
        },
        {
          icon: 'mdi-shopping',
          title: 'Products',
          to: '/product',
        },
        {
          icon: 'mdi-information',
          title: 'About Us',
          to: '/about',
        },
        {
          icon: 'mdi-phone-in-talk',
          title: 'Contact',
          to: '/contact',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
      icons: [
        {
          image: 'mdi-facebook',
          link: 'https://m.facebook.com/people/Semasa-Living/100069260500747/',
        },
        {
          image: 'mdi-email',
          link: 'https://m.facebook.com/people/Semasa-Living/100069260500747/',
        },
        {
          image: 'mdi-instagram',
          link: 'https://www.instagram.com/semasa.living/',
        },
      ],
    }
  },
  beforeCreate() {
    this.drawer = false
  },
  methods: {
    openWindow(link) {
      window.open(link)
    },
  },
}
</script>

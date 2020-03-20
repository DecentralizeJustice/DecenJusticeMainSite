<template>
  <v-container fluid class="ma-0 pa-0">
    <v-toolbar dark>
      <v-toolbar-title>Decentralize Justice</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
      color='grey darken-3'
      class="hidden-md-and-up" @click.stop="drawer = !drawer">
          <v-icon dark>mdi-menu</v-icon>
      </v-btn>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn elevation='0'  v-bind:input-value="page.link==current"
          v-for="page in pages"
          :key="page.title" :to="page.link">

            {{page.title}}

        </v-btn>
        <v-btn elevation='0' href="https://github.com/DecentralizeJustice">
            Github
        </v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <v-navigation-drawer
        v-model="drawer"
        absolute
        temporary
        app
        dark
      >
      <v-list dense>

        <v-list-item
          v-for="page in pages"
          :key="page.title"
          :to="page.link"
          link
        >
          <v-list-item-content>
            <v-list-item-title>{{page.title}}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>

        <!-- <v-list class="pt-0" dense>
          <v-divider></v-divider>
          <v-list-tile
            class="mt-2"
          >
            <v-list-tile-content style="font-size: 2em;">

            </v-list-tile-content>
          </v-list-tile>
        </v-list> -->
  </v-navigation-drawer>
</v-container>
</template>

<script>
export default {
  name: 'toolBar',
  props: {

  },
  data: () => ({
    pages: [
      { title: 'Projects', link: '/projects' },
      { title: 'About', link: '/about' }
    ],
    drawer: null,
    current: ''
  }),
  watch: {
    $route (to, from) {
      this.current = String(to.name)
    }
  }
}
</script>

<style scoped>
a{text-decoration: none;
color:white;}
</style>

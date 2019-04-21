<template>
  <div>
    <v-toolbar>
      <v-toolbar-side-icon class="hidden-md-and-up" @click.stop="drawer = !drawer"></v-toolbar-side-icon >
      <v-toolbar-title>Decentralize Justice</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn flat  v-bind:input-value="page.link==current"
          v-for="page in pages"
          :key="page.title" :to="page.link">

            {{page.title}}

        </v-btn>
        <v-btn flat href="https://github.com/DecentralizeJustice/project-Management">
            Github
        </v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <v-navigation-drawer
        v-model="drawer"
        absolute
        temporary
      >
        <v-list class="pt-0" dense>
          <v-divider></v-divider>
          <v-list-tile
            v-for="page in pages"
            :key="page.title"
            :to="page.link"
            class="mt-2"
          >
            <v-list-tile-content style="font-size: 2em;">
              {{page.title}}
            </v-list-tile-content>
          </v-list-tile>
        </v-list>
  </v-navigation-drawer>
</div>
</template>

<script>
export default {
  name: 'toolBar',
  props: {

  },
  data: () => ({
    pages: [
      { title: 'Projects', link: '/projects' },
      { title: 'About', link: '/about' },
      { title: 'Blog', link: '/blog' }
      // { title: 'Multisig Crypto', link: 'multisig' },
      // { title: 'R and D', link: 'randd' },
      // { title: 'Operations', link: 'operations' }
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

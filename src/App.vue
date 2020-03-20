<template>
  <v-app dark>
    <toolbar/>
    <v-content>
      <router-view/>
    </v-content>
  </v-app>
</template>

<script>
import toolbar from '@/components/toolBar.vue'
export default {
  name: 'App',
  components: {
    toolbar
  },
  data: () => ({
    //
  })
}
</script>

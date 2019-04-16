<template>
  <div>
    <toolBar/>
    <v-container fluid text-xs-center grid-list-xl>
      <v-layout
        justify-center row
        wrap class="my-5"
        align-center fill-height
      >
        <v-flex xs12 class="my-3">
          <div class="text-xs-center">
            <h2 class="headline">Here are our current projects:</h2>
          </div>
        </v-flex>

        <v-flex xs12 md4  v-for="(item, key) in items" :key="item.id">
          <v-card>
             <v-img
               v-bind:src="item.photo"
               aspect-ratio="2"
             ></v-img>
           <v-card-title primary-title class="justify-center">
             <div>
               <h3 class="headline mb-0">{{ key }}</h3>
             </div>
           </v-card-title>
           <v-card-actions class="justify-center">
             <v-btn flat color="orange" v-bind:href="item.link">{{ item.button }}</v-btn>
           </v-card-actions>
         </v-card>
        </v-flex>

      </v-layout>
    </v-container>
  </div>
</template>
<script>
import toolBar from '@/components/toolBar.vue'
export default {
  name: 'projects',
  components: {
    toolBar
  },
  data () {
    return {
      items: {
        'Multisig Crypto': { button: 'Explore', link: 'https://www.multisigcrypto.com/', photo: 'https://res.cloudinary.com/dylevfpbl/image/upload/v1555187114/decenMain/tech.jpg' },
        'Plastic Key Storage': { button: 'Explore', link: 'https://plastickeystorage.com', photo: 'https://res.cloudinary.com/dylevfpbl/image/upload/v1555187300/decenMain/plastic.jpg' },
        'Keys By Any Means': { button: 'Explore', link: 'https://keysbyanymeans.com/', photo: 'https://res.cloudinary.com/dylevfpbl/image/upload/v1555191944/decenMain/keystack.jpg' }

      }
    }
  }
}
</script>

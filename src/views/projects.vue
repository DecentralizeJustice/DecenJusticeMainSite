<template>
  <div>
    <v-flex xs12 class="ma-0 pa-0 first">
        <div class="text-xs-left center"
          v-bind:style="{color:'#8bd6ed',width:'75vw','letter-spacing':'.01em',
          'font-size':bannerfontSize,position:'relative'}">

          Our apps solve <span style="text-decoration: underline;font-weight:bold;">real</span> problems that
          <span style="text-decoration: underline;font-weight:bold;">actual</span> people have with using decentralized tech

        </div>
    </v-flex>
    <sect   v-for="item in data" :key="item.title"
        v-bind:sectObject="item" />

  </div>
</template>
<script>
import sect from '@/components/projects/sect.vue'
export default {
  name: 'projects',
  components: {
    sect
  },
  data () {
    return {
      data: [
        {
          title: 'Guiding Wallet',
          text: `Guiding Wallet aims to be the easiest and most helpfull wallet for people to use crypto. It has
          walkthrough videos, detailed courses, and secure software that guide your through the entire cryptocurrency process.
          It is like having experts in the room with you guiding you through out the crypto process.`,
          buttonText: 'Explore',
          odd: true,
          pageLink: 'https://guidingwallet.app/',
          backpic: 'https://res.cloudinary.com/dylevfpbl/image/upload/v1555187114/decenMain/tech.jpg',
          icon: 'https://res.cloudinary.com/dylevfpbl/image/upload/v1555796950/decenMain/undraw_interaction_design_odgc.svg'
        }
      ]
    }
  },
  computed: {
    bannerfontSize () {
      switch (this.$vuetify.breakpoint.name) {
        case 'sm': return '3em'
        case 'xs': return '2em'
        default: return '5em'
      }
    }
  }
}
</script>
<style scoped>

.first{
  height: 80vh;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-image: url('https://res.cloudinary.com/dylevfpbl/image/upload/v1555552411/decenMain/tech6.jpg');
}

.center{
  margin: 0;
  position: relative;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>

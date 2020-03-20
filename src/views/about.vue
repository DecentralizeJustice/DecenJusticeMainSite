<template>
  <v-container fluid class="pa-0">
    <v-row no-gutters class="ma-0 pa-0 first">
        <div class="text-xs-left center white--text ma-3 pa-3"
          v-bind:style="{width:'80vw','letter-spacing':'.01em','font-size':bannerfontSize,position:'relative'}">
          We create apps that <span style="text-decoration: underline;font-weight:bold;">empower</span> people
          to use the full potential of <span style="text-decoration: underline;font-weight:bold;">decentralized tech</span>
        </div>
    </v-row>

    <v-row no-gutters class="ma-0 pa-0">
    <textSect v-for="item in data" :key="item.title"
        v-bind:sectObject="item"/>
        </v-row>
  </v-container>
</template>
<script>
import textSect from '@/components/about/textSect.vue'
export default {
  name: 'about',
  components: {
    textSect
  },
  data () {
    return {
      data: [
        {
          title: 'What Drives Us',
          text: `We first got involved in crypto in 2014 by building mining rigs. To be in the space at this time required a
                  vast understanding of technology. Since then we have seen the crypto consumer space grow at
                  an exponential rate. Although the exponential for decentralized technologies has grown
                  since then, the tooling has not kept up with this growth. Most of the tools that exist
                  today are too advanced to be safe or to simple to be powerful. We are
                  working to bridge this gap with targeted applications that aim to empower,
                  not overwhelm or limit, users of decentralized technologies.`,
          svgLink: 'https://res.cloudinary.com/dylevfpbl/image/upload/v1555482590/decenMain/undraw_bitcoin2_ave7.svg',
          parraLink: 'https://res.cloudinary.com/dylevfpbl/image/upload/v1555450301/decenMain/mining-2648005_960_720.jpg'
        },
        {
          title: 'Who We Are',
          text: `Donely Gunn founded Decentralize Justice after the crypto bull run of 2017.
                  Donely has shown a passion for trying to improve society with technology since
                  a young age and has spent their life perfecting that craft. They first got
                  involved with crypto in high school via bitcoin mining, and they later saw major
                  issues in the usability of crypto and sought to solve a lot of these issues with Decentralize Justice.`,
          svgLink: 'https://res.cloudinary.com/dylevfpbl/image/upload/v1555482893/decenMain/vectorpaint.svg',
          parraLink: 'https://res.cloudinary.com/dylevfpbl/image/upload/v1555565441/decenMain/codenonblur.jpg'
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
  background-image: url("https://res.cloudinary.com/dylevfpbl/image/upload/v1555400445/decenMain/techblack_2.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.second{
  background-image: linear-gradient(120deg, #a1c4fd 0%, #c2e9fb 100%);
}
.third{
  background-color: #b1bfd8;
  background-image: linear-gradient(315deg, #b1bfd8 0%, #6782b4 74%);
}
.center{
  margin: 0;
  position: relative;
  top: 50%;
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
}

</style>

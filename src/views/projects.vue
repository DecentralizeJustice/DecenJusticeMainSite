<template>
  <div>
    <toolBar/>
    <v-flex xs12 class="ma-0 pa-0 first">
        <div class="text-xs-left center"
          v-bind:style="{color:'#8bd6ed',width:'75vw','letter-spacing':'.01em',
          'font-size':bannerfontSize,position:'relative'}">

          Our apps solve <span style="text-decoration: underline;font-weight:bold;">real</span> problems that
          <span style="text-decoration: underline;font-weight:bold;">actual</span> people have with using decentralized tech

        </div>
    </v-flex>
    <sect   v-for="item in data" :key="item.id"
        v-bind:sectObject="item" />

    <!-- <v-flex xs12 class="ma-0 pa-0 even">
      <v-layout row wrap>
        <v-flex xs6 style="height:100%;">
          <div class="" style="width:50vw;letter-spacing:.01em;font-size: 4.5em;color: white;position:relative;
            left: 5vw;
            top: 10vh;
            font-weight:bold;
            "
          >Plastic Key Storage</div>
          <div class="" style="width:44vw;font-size: 175%;color: white;position:relative;
            left: 4vw;
            top: 18vh;
            text-align: left;
            color: black;"
          >
            Plastic materials create a new option for crypto keys backup. It is
            <span style="font-weight:bold;">cheaper and easier</span> to use than metal backups.
            It is also more <span style="font-weight:bold;">durable</span> than writing your seed on paper.
             Plastic key storage methods will help more people secure their crypto keys.

        </div>
        <a href='https://plastickeystorage.com/' target="_blank"
        ><button  class="bttn-simple bttn-lg" style="position:relative;
          left: 21vw;
          top: 24vh;
          background-color: #58B1DB;
        "
        >Explore</button></a>

        </v-flex>
        <v-flex xs6 class="background secondp">
        </v-flex>
        </v-layout>
    </v-flex>

    <v-flex xs12 class="ma-0 pa-0 odd">
      <v-layout row wrap>
        <v-flex xs6 style="" class="background thirdp">
        </v-flex>
        <v-flex xs6 style="height:100%;">
          <div class="" style="width:50vw;letter-spacing:.01em;font-size: 4.5em;color: white;position:relative;
            left: 9vw;
            top: 10vh;
            font-weight:bold;
            "
          >Multisig Crypto</div>
          <div class="" style="width:44vw;font-size: 175%;color: white;position:relative;
            left: 4vw;
            top: 18vh;
            text-align: left;
            color: black;"
          >
            Multisignature is  the most <span style="font-weight:bold;">secure</span> way to use crypto. This technology
            has been kept beyond the reach of most consumers due to its complexity. Multisig Crypto is a wallet that will
            bring this technology from just the experts to <span style="font-weight:bold;">everyone</span>.
        </div>
        <a href='https://www.multisigcrypto.com/' target="_blank"
        ><button  class="bttn-simple bttn-lg" style="position:relative;
          left: 21vw;
          top: 24vh;
          background-color: #5D76A1;
        "
        >Explore</button></a>
        </v-flex>
        </v-layout>
    </v-flex> -->

  </div>
</template>
<script>
import toolBar from '@/components/toolBar.vue'
import sect from '@/components/projects/sect.vue'
export default {
  name: 'projects',
  components: {
    toolBar,
    sect
  },
  data () {
    return {
      data: [
        {
          title: 'Keys By Any Means',
          text: `Crypto Security and Usage is a unique issue, but the crypto space
          reccomends the same best practices to everyone. This app delivers a
          <span style="font-weight:bold;">customized</span> risk assessment and plan
          that allows you to own your keys in a way that works best for you.`,
          buttonText: 'Explore',
          odd: true,
          pageLink: 'https://keysbyanymeans.com/',
          backpic: 'https://res.cloudinary.com/dylevfpbl/image/upload/v1555191944/decenMain/keystack.jpg',
          icon: 'https://res.cloudinary.com/dylevfpbl/image/upload/v1555795100/decenMain/undraw_preferences_uuo2.svg'
        },
        {
          title: 'Plastic Key Storage',
          text: ` Plastic materials create a new option for crypto keys backup. It is
                  <span style="font-weight:bold;">cheaper and easier</span> to use than metal backups.
                  It is also more <span style="font-weight:bold;">durable</span> than writing your seed on paper.
                   Plastic key storage methods will help more people secure their crypto keys.`,
          buttonText: 'Explore',
          odd: false,
          pageLink: 'https://plastickeystorage.com/',
          backpic: 'https://res.cloudinary.com/dylevfpbl/image/upload/v1555546242/decenMain/cards-2179841_960_720.jpg',
          icon: 'https://res.cloudinary.com/dylevfpbl/image/upload/v1555792482/decenMain/undraw_profile_data_mk6k.svg'
        },
        {
          title: 'Multisig Crypto',
          text: `Multisignature is  the most <span style="font-weight:bold;">secure</span> way to use crypto. This technology
                  has been kept beyond the reach of most consumers due to its complexity. Multisig Crypto is a wallet that will
                  bring this technology from just the experts to <span style="font-weight:bold;">everyone</span>.`,
          buttonText: 'Explore',
          odd: true,
          pageLink: 'https://www.multisigcrypto.com/',
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

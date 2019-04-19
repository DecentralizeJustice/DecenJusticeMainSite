<template>
  <div>
    <toolBar/>
    <v-flex xs12 class="ma-0 pa-0 first">
        <div class="text-xs-left center"
          v-bind:style="{width:'75vw','letter-spacing':'.01em','font-size':bannerfontSize,position:'relative',left: '7vw'}">

          We create apps that <span style="text-decoration: underline;font-weight:bold;">empower</span> people
          to use the full potential of <span style="text-decoration: underline;font-weight:bold;">decentralized tech</span>

        </div>
    </v-flex>

    <firstsect/>
    <secondsect/>
    <thirdsect/>
        <!-- <v-flex xs12 class="ma-0 pa-0 third">
          <v-layout row wrap>
            <v-flex xs6 style="height:100%;">
              <div class="" style="width:40vw;letter-spacing:.01em;font-size: 4.5em;color: white;position:relative;
                left: 15vw;
                top: 10vh;
                font-weight:bold;
                "
              >Who We Are</div>
              <div class="" style="width:40vw;font-size: 175%;color: white;position:relative;
                left: 10vw;
                top: 8vw;
                text-align: left;
                color: black;"
              >
              Donely Gunn founded Decentralize Justice after the crypto bull run of 2017.
              Donely has shown a passion for trying to improve society with technology since
               a young age and has spent their life perfecting that craft.   They first got
                involved with crypto in high school via bitcoin mining, and they later saw major
              issues in the usability of crypto and sought to solve a lot of these issues with Decentralize Justice.
            </div>
            </v-flex>
            <v-flex xs6 style="height:80vh;">
                <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555482893/decenMain/vectorpaint.svg"
                  style="height:auto;width:30vw;position:relative;
                    left: 8vw;
                    top: 16vh;" >
            </v-flex>
            </v-layout>
        </v-flex>
        <v-parallax
        src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555447215/decenMain/mathsciencewhiz1.jpg">
        </v-parallax>

        <v-flex xs12 class="ma-0 pa-0 second">
          <v-layout row wrap>
            <v-flex xs6 style="height:100%;">
              <div class="" style="width:40vw;letter-spacing:.01em;font-size: 4.5em;color: white;position:relative;
                left: 18vw;
                top: 10vh;
                font-weight:bold;"
              >Reach Out</div>
              <div class="" style="width:50vw;font-size: 1.7em;position:relative;
                left: 8vw;
                top: 7vw;
                text-align: left;
                color: #09093B;"
              >Building community is vital for any project. If you have any questions, concerns, or just want
                  to see what we are up to, follow us on any platform below and reach out to us.
            </div>
            <a href="https://www.reddit.com/r/DecentralizeJustice" target="_blank">
            <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555450247/decenMain/Reddit_Mark_OnDark.png"
              style="height:auto;width:30%;position:relative;
                left: 10vw;
                top: 10vh;" >
              </a>
                <a href="https://twitter.com/DecenJustice" target="_blank">
                <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555472356/decenMain/Twitter_Logo_Blue.png"
                  style="height:auto;width:40%;position:relative;
                    left: 14vw;
                    top: 15vh;">
                  </a>
            </v-flex>
            <v-flex xs6 style="height:80vh;">
                <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555483001/decenMain/undraw_social_thinking_7ule.svg"
                  style="height:auto;width:50vh;position:relative;
                    left: 10vw;
                    top: 20vh;" >
            </v-flex>
          </v-layout>

        </v-flex> -->

  </div>
</template>
<script>
import toolBar from '@/components/toolBar.vue'
import firstsect from '@/components/about/firstsect.vue'
import secondsect from '@/components/about/secondsect.vue'
import thirdsect from '@/components/about/thirdsect.vue'
export default {
  name: 'about',
  components: {
    toolBar,
    firstsect,
    secondsect,
    thirdsect
  },
  computed: {
    bannerfontSize () {
      switch (this.$vuetify.breakpoint.name) {
        case 'sm': return '3em'
        case 'xs': return '2em'
        default: return '5em'
      }
    },
    sectionheight () {
      switch (this.$vuetify.breakpoint.name) {
        case 'sm': return '125vh'
        case 'xs': return '125vh'
        default: return '80vh'
      }
    },
    titlefontsize () {
      switch (this.$vuetify.breakpoint.name) {
        case 'md': return '300%'
        case 'sm': return '300%'
        case 'xs': return '125%'
        default: return '400%'
      }
    },
    bodyfontsize () {
      switch (this.$vuetify.breakpoint.name) {
        case 'md': return '140%'
        case 'sm': return '300%'
        case 'xs': return '125%'
        default: return '155%'
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

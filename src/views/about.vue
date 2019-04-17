<template>
  <div>
    <toolBar/>

        <v-flex xs12 class="ma-0 pa-0 first">

          <div class="text-xs-left center ml-5" style="  ">
            <div class="" style="width:63%;letter-spacing: .01em;font-size: 4.5em">We create apps that empower people
              to use the full potential of decentralized technology</div>
          </div>
        </v-flex>

        <v-flex xs12 class="ma-0 pa-0 second">
          <v-layout row wrap>
            <v-flex xs6 style="height:100%;">
              <div class="" style="width:40vw;letter-spacing:.01em;font-size: 4.5em;color: white;position:relative;
                left: 10vw;
                top: 10vh;
                font-weight:bold;
                text-decoration: underline;"
              >What Drives Us</div>
              <div class="" style="width:50vw;font-size: 1.7em;position:relative;
                left: 5vw;
                top: 10vw;
                text-align: left;
                color: #09093B;"
              >
              We first got involved in crypto in 2014 by building mining rigs. To be in the space at this time required a
              vast understanding of technology. Since then we have seen the crypto consumer space grow at
              an exponential rate. Although the exponential for decentralized technologies has grown
              since then, the tooling has not kept up with this growth. Most of the tools that exist
              today are too advanced to be safe or to simple to be powerful. We are
               working to bridge this gap with targeted applications that aim to empower,
               not overwhelm or limit, users of decentralized technologies.
            </div>
            </v-flex>
            <v-flex xs6 style="height:80vh;">
                <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555482590/decenMain/undraw_bitcoin2_ave7.svg"
                  style="height:auto;width:20vw;position:relative;
                    left: 18vw;
                    top: 20vh;" >
            </v-flex>
          </v-layout>
        </v-flex>

        <v-parallax
        src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555450301/decenMain/mining-2648005_960_720.jpg">
        </v-parallax>

        <v-flex xs12 class="ma-0 pa-0 third">
          <v-layout row wrap>
            <v-flex xs6 style="height:100%;">
              <div class="" style="width:40vw;letter-spacing:.01em;font-size: 4.5em;color: white;position:relative;
                left: 3vw;
                top: 10vh;
                font-weight:bold;
                text-decoration: underline;"
              >Who We Are</div>
              <div class="" style="width:40vw;font-size: 175%;color: white;position:relative;
                left: 3vw;
                top: 8vw;
                text-align: left;
                color: black;"
              >Donely Gunn founded Decentralize Justice after the crypto bull run of 2017.
              Donely has shown a passion for trying to improve society with technology since
               a young age and has spent thier life perfecting that craft.   They first got
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
                left: 10vw;
                top: 10vh;
                font-weight:bold;
                text-decoration: underline;"
              >Reach Out</div>
              <div class="" style="width:50vw;font-size: 1.7em;position:relative;
                left: 5vw;
                top: 8vw;
                text-align: left;
                color: #09093B;"
              >Building community is vital for any project. If you have any questions, concerns, or just want
                  to see what we are up to, follow us on any platform below and reach out to us.
            </div>
            <a href="https://www.reddit.com/r/DecentralizeJustice" target="_blank">
            <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555450247/decenMain/Reddit_Mark_OnDark.png"
              style="height:auto;width:30%;position:relative;
                left: 2vw;
                top: 10vh;" >
              </a>
                <a href="https://twitter.com/DecenJustice" target="_blank">
                <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555472356/decenMain/Twitter_Logo_Blue.png"
                  style="height:auto;width:40%;position:relative;
                    left: 4vw;
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

        </v-flex>

        <v-parallax
        src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555472641/decenMain/social-media-1795578_960_720.jpg">
        </v-parallax>

  </div>
</template>
<script>
import toolBar from '@/components/toolBar.vue'

export default {
  name: 'about',
  components: {
    toolBar },
  data () {
    return {
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
  height: 80vh;
  background-image: linear-gradient(120deg, #a1c4fd 0%, #c2e9fb 100%);
}
.third{
  height: 80vh;
  background-color: #b1bfd8;
  background-image: linear-gradient(315deg, #b1bfd8 0%, #6782b4 74%);
}
.center{
  margin: 0;
  position: relative;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>

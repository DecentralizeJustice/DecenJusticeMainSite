<template>
  <div>
    <toolBar/>
    <v-container fluid text-xs-center grid-list-xl class="ma-0 pa-0">
      <v-layout
        justify-center row
        wrap class="ma-0 pa-0"
        align-center fill-height
      >
        <v-flex xs12 class="ma-0 pa-0 first">
          <div class="text-xs-left center ml-5" style="  ">
            <div class="" style="width:63%;letter-spacing: .03em;font-size: 4.5em">We create apps that empower people
              to use the full potential of decentralized technology.</div>
          </div>
        </v-flex>

        <v-flex xs12 class="ma-0 pa-0 second">
          <v-layout row wrap>
            <v-flex xs6 style="height:100%;">
              <div class="" style="width:40vw;letter-spacing:.01em;font-size: 4.5em;color: black;position:relative;
                left: 10vw;
                top: 10vh;"
              >What Drives Us</div>
              <div class="" style="width:50vw;font-size: 1.7em;color: white;position:relative;
                left: 5vw;
                top: 10vw;
                text-align: left;
                color: black;"
              >We first got involved in crypto in 2014. To be in the space at this time required a
              vast understanding of technology. Since then we have seen the crypto space grow at
              an exponential rate. Although the exponential for decentralized technologies has grown
              since then, the tooling has not kept up with this growth. Most of the tools that exist
              today are too advanced to be safe or to simple to be powerful. Decentralize Justice is
               working to bridge this gap with targeted applications that aim to empower,
               not overwhelm or limit, users of decentralized technologies.
            </div>
            </v-flex>
            <v-flex xs6 style="height:80vh;">
                <img src="https://cdn.pixabay.com/photo/2015/09/05/20/02/coding-924920_960_720.jpg"
                  style="height:auto;width:80%;position:relative;
                    left: 2vw;
                    top: 20vh;" >
            </v-flex>
          </v-layout>

        </v-flex>

      </v-layout>
    </v-container>
  </div>
</template>
<script>
import toolBar from '@/components/toolBar.vue'
export default {
  name: 'about',
  components: {
    toolBar
  },
  data () {
    return {
    }
  }
}
</script>
<style scoped>
.first{
  height: 85vh;
  background-image: url("https://res.cloudinary.com/dylevfpbl/image/upload/v1555400445/decenMain/techblack_2.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.second{
  height: 80vh;
  background-color: #ffffff;
  background-image: linear-gradient(315deg, #ffffff 0%, #d7e1ec 74%);
}
.center{
  margin: 0;
  position: relative;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

</style>

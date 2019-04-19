<template>
<div>
  <div class='hidden-sm-and-down'>
      <v-flex xs12 class="ma-0 pa-0 second" style="height:100vh;">
        <v-layout row wrap>
          <v-flex xs9 style="height:100vh;">

            <div style="width:100%;
            position:relative;left: 2%;top: 8%;">

              <div  class="text-xs-center"
                style="width:70%;font-size:10vh;color: white;
                position:relative;left: 14%;top: 80%;font-weight:bold;"
              >What Drives Us</div>

                <div
                  style="width: 60vw;font-size: 3.5vh;
                  position:relative;left:10%;top: 4vh;
                  color: #09093B;text-align:left;" v-html="main"
                >
               </div>
            </div>
          </v-flex>
          <v-flex xs3  style="height:100vh;">
              <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555482590/decenMain/undraw_bitcoin2_ave7.svg"
                style="height:40vh;width:auto;position:relative;
                  left: 0%;
                  top: 30vh;" >
          </v-flex>
        </v-layout>
      </v-flex>
      <v-parallax style="height:50vh;"
      src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555450301/decenMain/mining-2648005_960_720.jpg">
      </v-parallax>
  </div>

  <v-flex xs12 class="ma-0 pa-0 second hidden-md-and-up">

      <div  class="text-xs-center"
        style="width:100%;font-size:6vh;color: white;
        position:relative;top: 3vh;font-weight:bold;"
      >What Drives Us</div>

        <div
          style="width: 100vw;font-size: 3vh;
          position:relative;top: 4vh;
          color: #09093B;text-align:left;padding:3%;" v-html="main"
        >
       </div>

    <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555482590/decenMain/undraw_bitcoin2_ave7.svg"
      style="height:auto;width:50vw;position:relative;margin-top:5vh;margin-bottom:5vh;" class="center">
  </v-flex>

</div>
</template>
<script>
export default {
  name: 'firstsect',
  components: {

  },
  data () {
    return {
      main: `We first got involved in crypto in 2014 by building mining rigs. To be in the space at this time required a\
              vast understanding of technology. Since then we have seen the crypto consumer space grow at\
              an exponential rate. Although the exponential for decentralized technologies has grown\
              since then, the tooling has not kept up with this growth. Most of the tools that exist\
              today are too advanced to be safe or to simple to be powerful. We are\
              working to bridge this gap with targeted applications that aim to empower,\
              not overwhelm or limit, users of decentralized technologies.`
    }
  },
  computed: {
  }
}
</script>
<style scoped>

.second{
  background-image: linear-gradient(120deg, #a1c4fd 0%, #c2e9fb 100%);
}

.center{
  position: relative;
  left: 50%;
  -ms-transform: translateX(-50%);
  transform: translateX(-50%);
}

</style>

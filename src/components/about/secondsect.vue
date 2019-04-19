<template>
<div>
  <div class='hidden-sm-and-down'>
      <v-flex xs12 class="ma-0 pa-0 second" style="height:80vh;">
        <v-layout row wrap>
          <v-flex xs9>

            <div style="width:100%;
            position:relative;left: 2%;top: 8%;">

              <div  class="text-xs-center"
                style="width:70%;font-size:10vh;color: white;
                position:relative;left: 14%;top: 80%;font-weight:bold;"
              >Who We Are</div>

                <div
                  style="width: 60vw;font-size: 3.5vh;
                  position:relative;left:10%;top: 4vh;
                  color: #09093B;text-align:left;" v-html="main"
                >
               </div>
            </div>
          </v-flex>
          <v-flex xs3>
              <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555482893/decenMain/vectorpaint.svg"
                style="height:40vh;width:auto;position:relative;
                  left: 0%;
                  top: 30vh;" >
          </v-flex>
        </v-layout>
      </v-flex>
      <v-parallax style="height:50vh;"
      src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555707015/decenMain/mathsciencewhiz1_1.jpg">
      </v-parallax>
  </div>

  <v-flex xs12 class="ma-0 pa-0 second hidden-md-and-up">

      <div  class="text-xs-center"
        style="width:100%;font-size:6vh;color: white;
        position:relative;top: 3vh;font-weight:bold;"
      >Who We Are</div>

        <div
          style="width: 100vw;font-size: 3vh;
          position:relative;top: 4vh;
          color: #09093B;text-align:left;padding:3%;" v-html="main"
        >
       </div>

    <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555482893/decenMain/vectorpaint.svg"
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
      main: `Donely Gunn founded Decentralize Justice after the crypto bull run of 2017.
              Donely has shown a passion for trying to improve society with technology since
              a young age and has spent their life perfecting that craft.   They first got
              involved with crypto in high school via bitcoin mining, and they later saw major
              issues in the usability of crypto and sought to solve a lot of these issues with Decentralize Justice.`
    }
  },
  computed: {
  }
}
</script>
<style scoped>

.second{
  background-image: linear-gradient(120deg, #e0c3fc 0%, #8ec5fc 100%);
}

.center{
  position: relative;
  left: 50%;
  -ms-transform: translateX(-50%);
  transform: translateX(-50%);
}

</style>

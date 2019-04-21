<template>
<div>
  <div class='hidden-sm-and-down'>
      <v-flex xs12 class="ma-0 pa-0 second" v-bind:style="{ 'height': height }">
        <v-layout row wrap>
          <v-flex xs9 v-bind:style="{ 'height': height }">

            <div style="width:100%;
            position:relative;left: 2%;top: 8%;">

              <div  class="text-xs-center"
                style="width:70%;font-size:10vh;color: white;
                position:relative;left: 14%;top: 80%;font-weight:bold;" v-html="sectObject.title"
              ></div>

                <div
                  style="width: 60vw;font-size: 3.5vh;
                  position:relative;left:10%;top: 4vh;
                  color: #09093B;text-align:left;" v-html="sectObject.text"
                >
               </div>
            </div>
          </v-flex>
          <v-flex xs3 v-bind:style="{ 'height': height }">
              <img :src="sectObject.svgLink" class="centerY"
                style="height:40%;width:auto;position:relative;" >
          </v-flex>
        </v-layout>
      </v-flex>
      <v-parallax style="height:50vh;"
      :src="sectObject.parraLink">
      </v-parallax>
  </div>

  <v-flex xs12 class="ma-0 pa-0 second hidden-md-and-up">

      <div  class="text-xs-center"
        style="width:100%;font-size:6vh;color: white;
        position:relative;top: 3vh;font-weight:bold;"
        v-html="sectObject.title"
      ></div>

        <div
          style="width: 100vw;font-size: 3vh;
          position:relative;top: 4vh;
          color: #09093B;text-align:left;padding:3%;" v-html="sectObject.text"
        >
       </div>

    <img :src="sectObject.svgLink"
      style="height:auto;width:50vw;position:relative;margin-top:5vh;margin-bottom:5vh;" class="center">
  </v-flex>

</div>
</template>
<script>
export default {
  name: 'textSect',
  props: ['sectObject'],
  components: {

  },
  data () {
    return {
    }
  },
  computed: {
    height: function () {
      if (this.sectObject.short === true) {
        return '80vh'
      }
      return '90vh'
    }
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
.centerY{
  position: relative;
  top: 50%;
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
}
</style>

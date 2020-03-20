<template>
    <v-col
    cols='12'
    style="height:100%;background-color: #1565C0;"
      >
        <div  class="text-center white--text display-3 font-weight-medium ma-5"
          style="" v-html="sectObject.title"
        ></div>
        <div
        class="text-left white--text headline font-weight-regular ma-5"
          style="" v-html="sectObject.text"
        >
       </div>
       <img :src="sectObject.svgLink"
         style="height:auto;width:25vw;" class="center mb-3">
       <v-parallax style="height: 50vh;" :src="sectObject.parraLink"></v-parallax>
    </v-col>
  <!-- <v-flex xs12 class="ma-0 pa-0 second hidden-md-and-up">

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
  </v-flex> -->
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

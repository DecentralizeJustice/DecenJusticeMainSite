<template>
<div>

  <v-flex xs12 class="ma-0 pa-0 second hidden-md-and-up">

      <div  class="text-xs-center"
        style="width:100%;font-size:6vh;color: white;
        position:relative;top: 3vh;font-weight:bold;"
      >Reach Out</div>

        <div
          style="width: 100vw;font-size: 3vh;
          position:relative;top: 4vh;
          color: #09093B;text-align:left;padding:3%;" v-html="main"
        >
       </div>
       <div>
       <a href="https://twitter.com/DecenJustice">
       <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555472356/decenMain/Twitter_Logo_Blue.png"
         style="height:auto;width:40%;position:relative;
           left: 5vw;
           top: 0vh;">
         </a>
         <a href="https://www.reddit.com/r/DecentralizeJustice" target="_blank">
         <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555450247/decenMain/Reddit_Mark_OnDark.png"
           style="height:auto;width:30%;position:relative;
             left: 12vw;
             top:-2vh;" >
           </a>
        </div>
  </v-flex>

</div>
</template>
<script>
export default {
  name: 'thirdsect',
  components: {

  },
  data () {
    return {
      main: `Building community is vital for any project. If you have any questions, concerns, or just want
          to see what we are up to, follow us on any platform below and reach out to us.`
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

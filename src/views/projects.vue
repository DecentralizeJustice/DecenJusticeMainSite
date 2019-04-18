<template>
  <div>
    <toolBar/>
    <v-flex xs12 class="ma-0 pa-0 first">
      <div class="text-xs-left center ml-5" style="  ">
        <div class="" style="width:63%;
        font-size: 4.5em;color:White;font-weight:bold;
        position:relative;left: 5vw;top: 10vh;">
          Cypherpunks Write Code <span style="font-size: .5em;"><br>-Cypherpunks Manifesto</span></div>
      </div>
    </v-flex>

    <v-flex xs12 class="ma-0 pa-0 third">
      <v-layout row wrap>
        <v-flex xs6 style="" class="background firstp">
        </v-flex>
        <v-flex xs6 style="height:100%;">
          <div class="" style="width:50vw;letter-spacing:.01em;font-size: 4.5em;color: white;position:relative;
            left: 5vw;
            top: 10vh;
            font-weight:bold;
            "
          >Keys By Any Means</div>
          <div class="" style="width:44vw;font-size: 175%;color: white;position:relative;
            left: 4vw;
            top: 18vh;
            text-align: left;
            color: black;"
          >
            Crypto Security and Usage is a deeply unique issue, but the crypto space
            reccomends the same best practices to everyone. This app delivers a
            <span style="font-weight:bold;">customized</span> risk assemsnt and plan
            that allows you to own your keys in a way that works best for you.
        </div>
        <v-btn color="info" style="position:relative;
          left: 21vw;
          top: 24vh;
        " href='https://keysbyanymeans.com/' target="_blank"
        >Explore</v-btn>
        </v-flex>
        </v-layout>
    </v-flex>

    <v-flex xs12 class="ma-0 pa-0 third">
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
            Crypto Security and Usage is a deeply unique issue, but the crypto space
            reccomends the same best practices to everyone. This app delivers a
            <span style="font-weight:bold;">customized</span> risk assemsnt and plan
            that allows you to own your keys in a way that works best for you.
        </div>
        <v-btn color="info" style="position:relative;
          left: 21vw;
          top: 24vh;
        " href='https://plastickeystorage.com/' target="_blank"
        >Explore</v-btn>
        </v-flex>
        <v-flex xs6 class="background secondp">
        </v-flex>
        </v-layout>
    </v-flex>

    <v-flex xs12 class="ma-0 pa-0 third">
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
            Crypto Security and Usage is a deeply unique issue, but the crypto space
            reccomends the same best practices to everyone. This app delivers a
            <span style="font-weight:bold;">customized</span> risk assemsnt and plan
            that allows you to own your keys in a way that works best for you.
        </div>
        <v-btn color="info" style="position:relative;
          left: 21vw;
          top: 24vh;
        " href='https://www.multisigcrypto.com/' target="_blank"
        >Explore</v-btn>
        </v-flex>
        </v-layout>
    </v-flex>

  </div>
</template>
<script>
import toolBar from '@/components/toolBar.vue'
export default {
  name: 'projects',
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
  height: 80vh;
  background-position: center; /* Center the image */
  background-repeat: no-repeat; /* Do not repeat the image */
  background-size: cover;
  background-image: url('https://res.cloudinary.com/dylevfpbl/image/upload/v1555546002/decenMain/abstract-art-background-633409.jpg');
}
.third{
  height: 80vh;
  background-image: radial-gradient(circle 248px at center, #16d9e3 0%, #30c7ec 47%, #46aef7 100%);
}
.background{
  background-position: center; /* Center the image */
  background-repeat: no-repeat; /* Do not repeat the image */
  background-size: cover;
}
.firstp{
  height:80vh;
  background-image: url('https://res.cloudinary.com/dylevfpbl/image/upload/v1555191944/decenMain/keystack.jpg');
}
.secondp{
  height:80vh;
  background-image: url('https://res.cloudinary.com/dylevfpbl/image/upload/v1555187300/decenMain/plastic.jpg');
}
.thirdp{
    height:80vh;
  background-image: url('https://res.cloudinary.com/dylevfpbl/image/upload/v1555187114/decenMain/tech.jpg')
}
</style>

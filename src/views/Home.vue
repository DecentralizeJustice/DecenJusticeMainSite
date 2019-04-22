<template>
  <v-container  text-xs-center fluid ma-0 pa-0 >
    <v-layout row wrap ma-0 pa-0>
      <v-flex xs12 ma-0 pa-0 hidden-sm-and-down style="overflow: hidden;">
        <video style="
        position: fixed;
        right: 0;
        bottom: 0;
        min-width: 100%;
        min-height: 100%;"
        src="https://res.cloudinary.com/dylevfpbl/video/upload/v1551009310/decenMain/yes.mp4" autoplay muted loop/>

        <v-flex class="title" md8 offset-xs2 pa-2 >
          <div class="display-4 white--text text-xs-center" >
            Decentralize Justice
          </div>
          <br>
          <div class="text-xs-center">
            <v-btn flat class="buttonOpt" to="/projects">Projects</v-btn>
            <v-btn flat class="buttonOpt" to="/about" >About</v-btn>
            <v-btn flat class="buttonOpt" href="https://www.decentralizejustice.com/blog">Blog</v-btn>
          </div>
        </v-flex>
      </v-flex>

      <v-flex xs12 ma-0 pa-0 hidden-md-and-up
      style="background-image: url('https://res.cloudinary.com/dylevfpbl/image/upload/v1555565441/decenMain/codenonblur.jpg');
      height:100vh;width:100vw;  background-repeat: no-repeat;
        background-size: cover; ">
        <v-flex class="title" xs12 pa-4 style="background-color: rgb(169,169,169,.9);">
          <div class="display-2 white--text text-xs-center" >
            Decentralize Justice
          </div>
          <br>
          <div class="text-xs-center">
            <v-btn flat class="buttonOpt" to="/projects">Projects</v-btn>
            <v-btn flat class="buttonOpt" to="/about" >About</v-btn>
            <v-btn flat class="buttonOpt" href="https://www.decentralizejustice.com/blog">Blog</v-btn>
          </div>
        </v-flex>
      </v-flex>
      </v-layout>
  </v-container>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'home',
  components: {

  }
}
</script>
<style scoped>
a{
  text-decoration: none;
  color:white;
}
.title{
  margin: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background-color: rgb(169,169,169,.9);
}
.buttonOpt {
  color:  white;
  font-size: 1.4rem;
  background-color: grey;
}

</style>

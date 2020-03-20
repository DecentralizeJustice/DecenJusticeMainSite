<template>
  <v-container  text-xs-center fluid ma-0 pa-0 >
    <v-row no-gutters>
      <v-col cols='12' class="hidden-sm-and-down" style="overflow: hidden;">
        <video style="
        position: fixed;
        right: 0;
        bottom: 0;
        min-width: 100%;
        min-height: 100%;"
        src="https://res.cloudinary.com/dylevfpbl/video/upload/v1551009310/decenMain/yes.mp4" autoplay muted loop/>
        <v-row no-gutters justify='center'>
        <v-col class="nametitle pa-5" text-center lg='6' md='7' >
          <div class="display-4 white--text text-center font-weight-medium" >
            Decentralize Justice
          </div>
          <br>
          <div class="text-center" >
            <v-btn class="buttonOpt mr-2" color='black' to="/projects">Projects</v-btn>
            <v-btn class="buttonOpt" color='black' to="/about" >About</v-btn>
          </div>
        </v-col>
        </v-row>
      </v-col>

      <v-col cols='12' ma-0 pa-0 class="hidden-md-and-up"
      style="background-image: url('https://res.cloudinary.com/dylevfpbl/image/upload/v1555565441/decenMain/codenonblur.jpg');
      height:100vh;width:100vw;  background-repeat: no-repeat;
        background-size: cover; ">
        <v-row no-gutters justify='center' align='center' style="height:100vh;">
        <v-col class="title" cols='12' pa-4 style="background-color: rgb(169,169,169,.9);">
          <div class="display-3 white--text text-center" >
            Decentralize Justice
          </div>
          <div class="text-center pa-2">
            <v-btn class="buttonOpt mr-2" color='black' to="/projects">Projects</v-btn>
            <v-btn class="buttonOpt"  color='black' to="/about" >About</v-btn>
          </div>
        </v-col>
        </v-row>
      </v-col>
      </v-row>
  </v-container>
</template>

<script>
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
.nametitle{
  border-radius: 25px;
  margin: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background-color: rgb(169,169,169,.95);
}
.buttonOpt {
  color:  white;
  font-size: 1.2rem;
}

</style>

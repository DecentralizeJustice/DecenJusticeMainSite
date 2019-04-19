<template>
<div>
    <v-flex xs12 class="ma-0 pa-0 second hidden-sm-and-down" style="height:80vh;">
      <v-layout row wrap>
        <v-flex md6 xs12 style="height:100vh;">

          <div style="width:100%;
          position:relative;left: 2%;top: 8%;">

            <div  class="text-xs-center"
              style="width:70%;font-size:400%;color: white;
              position:relative;left: 20%;top: 8%;font-weight:bold;"
            >What Drives Us</div>

              <div  class=""
                style="width: 100%;font-size: 200%;color: white;
                position:relative;left:15%;top: 10%;
                color: #09093B;text-align:left;"
              >
              We first got involved in crypto in 2014 by building mining rigs. To be in the space at this time required a
              vast understanding of technology. Since then we have seen the crypto consumer space grow at
              an exponential rate. Although the exponential for decentralized technologies has grown
              since then, the tooling has not kept up with this growth. Most of the tools that exist
              today are too advanced to be safe or to simple to be powerful. We are
               working to bridge this gap with targeted applications that aim to empower,
               not overwhelm or limit, users of decentralized technologies.
             </div>
          </div>
        </v-flex>
        <v-flex md6 xs12 style="height:25vh;">
            <img src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555482590/decenMain/undraw_bitcoin2_ave7.svg"
              style="height:auto;width:50%;position:relative;
                left: 25%;
                top: 50%;" >
        </v-flex>
      </v-layout>
    </v-flex>
    <v-parallax
    src="https://res.cloudinary.com/dylevfpbl/image/upload/v1555450301/decenMain/mining-2648005_960_720.jpg">
    </v-parallax>
</div>
</template>
<script>
export default {
  name: 'fbody',
  components: {

  }
}
</script>
<style scoped>

.second{
  background-image: linear-gradient(120deg, #a1c4fd 0%, #c2e9fb 100%);
}

.center{
  margin: 0;
  position: relative;
  top: 50%;
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
}

</style>

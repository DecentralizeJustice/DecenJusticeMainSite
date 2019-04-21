<template>
  <div>
    <toolBar/>
    <v-flex xs12 class="ma-0 pa-0 first">
        <div class="text-xs-left center"
          v-bind:style="{width:'75vw','letter-spacing':'.01em','font-size':bannerfontSize,position:'relative',left: '7vw'}">

          We create apps that <span style="text-decoration: underline;font-weight:bold;">empower</span> people
          to use the full potential of <span style="text-decoration: underline;font-weight:bold;">decentralized tech</span>

        </div>
    </v-flex>

    <firstsect/>
    <secondsect/>
    <thirdsect/>
  </div>
</template>
<script>
import toolBar from '@/components/toolBar.vue'
import firstsect from '@/components/about/firstsect.vue'
import secondsect from '@/components/about/secondsect.vue'
import thirdsect from '@/components/about/thirdsect.vue'
export default {
  name: 'about',
  components: {
    toolBar,
    firstsect,
    secondsect,
    thirdsect
  },
  computed: {
    bannerfontSize () {
      switch (this.$vuetify.breakpoint.name) {
        case 'sm': return '3em'
        case 'xs': return '2em'
        default: return '5em'
      }
    }
  }
}
</script>
<style scoped>

.first{
  height: 80vh;
  background-image: url("https://res.cloudinary.com/dylevfpbl/image/upload/v1555400445/decenMain/techblack_2.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.second{
  background-image: linear-gradient(120deg, #a1c4fd 0%, #c2e9fb 100%);
}
.third{
  background-color: #b1bfd8;
  background-image: linear-gradient(315deg, #b1bfd8 0%, #6782b4 74%);
}
.center{
  margin: 0;
  position: relative;
  top: 50%;
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
}

</style>

<template>
  <div>
    <v-flex xs12 >
      <v-layout row wrap style="height:80vh;"
        v-bind:class="{ 'ma-0': true, 'pa-0': true,'hidden-sm-and-down': true, 'odd': odd, 'even': !odd  }">
        <v-flex xs6
          v-bind:style="{'height':'100%', backgroundImage: 'url(' + sectObject.backpic + ')'}"
          v-bind:class="{ 'order-sm2': odd,'background': true  }">
        </v-flex>
          <v-flex xs6 style="height:100%;text-align: center;"
            v-bind:class="{ 'order-sm1': odd,  }">
            <div style="width:100%;letter-spacing:.01em;
            font-size:3vw;position:relative;top: 10vh;
              font-weight:bold;text-align: center;
              "
              v-bind:class="{ 'titleOdd': odd,'titleEven': !odd, 'text-xs-center': true }"
              v-html="sectObject.title"
            ></div>
            <div style="width:80%;font-size: 175%;position:relative;
              top: 18vh;
              left:10%;
              text-align: left;"
              v-bind:class="{ 'textOdd': odd,'textEven': !odd  }"
              v-html="sectObject.text"
            >
          </div>
          <a :href='sectObject.pageLink'
          >
            <button  style="position:static; margin-top:25%;"
            v-html="sectObject.buttonText"
            v-bind:class="{ 'bttn-simple': true, 'bttn-lg': true,
            'buttonOdd': odd,'buttonEven': !odd  }"
            ></button>
          </a>
        </v-flex>
        </v-layout>
    </v-flex>

    <v-flex xs12
      v-bind:class="{ 'ma-0': true, 'pa-0': true,'hidden-md-and-up': true, 'odd': odd, 'even': !odd  }" >
      <div  v-bind:class="{ 'titleOdd': odd,'titleEven': !odd, 'text-xs-center': true }"
        style="width:100%;font-size:6vh;
        position:relative;top: 3vh;font-weight:bold;padding:2%;"
        v-html="sectObject.title"
      ></div>

      <div v-bind:class="{ 'textOdd': odd,'textEven': !odd  }"
        style="width: 100vw;font-size: 3vh;
        position:relative;top: 4vh;
        text-align:left;padding:3%;" v-html="sectObject.text"
      >
     </div>

      <a :href='sectObject.pageLink'
       >
         <button  style="
           margin-top:5vh;margin-bottom:5vh;
         "
         v-html="sectObject.buttonText"
         v-bind:class="{ 'bttn-simple': true, 'center':true, 'bttn-lg': true,
          'buttonOdd': odd,'buttonEven': !odd  }"
         ></button>
      </a>
      <img :src="sectObject.icon"
       style="height:auto;width:50vw;position:relative;display:block;padding-bottom:5vh;" class="center">
    </v-flex>
  </div>
</template>
<script>
export default {
  name: 'sect',
  props: ['sectObject'],
  components: {
  },
  data () {
    return {
    }
  },
  computed: {
    odd: function () {
      if (this.sectObject.odd === true) {
        return true
      }
      return false
    }
  }
}
</script>
<style scoped>

.odd{
  background-image: linear-gradient(to top, #fff1eb 0%, #ace0f9 100%);
}
.even{
  background-image: linear-gradient(to top, #6a85b6 0%, #bac8e0 100%);
}
.textOdd{
  color: #09093B;
}
.textEven{
  color: #09093B;
}
.titleOdd{
  color:white;
}
.titleEven{
  color:white;
}
.buttonOdd{
  background-color: #5D76A1;
}
.buttonEven{
  background-color: #58B1DB
}

.background{
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.center{
  position: relative;
  left: 50%;
  -ms-transform: translateX(-50%);
  transform: translateX(-50%);
}
</style>

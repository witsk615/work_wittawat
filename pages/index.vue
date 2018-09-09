<template>
<v-parallax src="/image/1.jpg" >
  <div>
    <nuxt-link to="/login">
    <center>
       <div class="text-xs-center">
    <v-btn round color="primary" dark>LOGIN</v-btn>
  </div>
    </center> 
    </nuxt-link><br>
    <router-link :to="{ path: '/Profile'}" replace><center>
      <div class="text-xs-center">
        <v-btn round color="primary" dark>PROFILE</v-btn>
      </div>
    </center>
    </router-link><br>
  </div>

</v-parallax>
</template>
<script>
  export default {
    data () { 
      return {
        items: [
          {
            src: '/image/1.jpg'
          },
          {
            src: '/image/2.jpg'
          },
          {
            src: '/image/bb.jpg'
          },
          {
            src: '/image/phone.jpg'
          }
        ]
      }
    }
  }
</script>
<script>
export default {
  layout : "public",
  data() {
    return {
      id: 1,
    }
  },
}
</script>
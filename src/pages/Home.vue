<template>

  <div>
    <h1>Home page</h1>
    <a href="/cars">Go to Cars page</a>

    <Home1></Home1>
    <Home2></Home2>
  </div>



</template>

<script>
import Home1 from './Home1'
import Home2 from './Home2'

export default {
  components: {
    Home1,
    Home2,
  },

  mounted() {
    //console.log('HOME component mounted')
  },

  methods: {

    hello: function () {
      console.log('hello from home page')
    }

  }

}
</script>

<style scoped></style>

<template>

  <div style="border:2px solid dodgerblue; padding:15px">
    <h3>Home2 component</h3>
  </div>

</template>

<script>
export default {

  mounted() {
    this.$root.$on('eventExampleEmit', (item, response) => {
      console.log('eventExampleEmit catch in Home2 - ' + item + response)
    })
    console.log('Home2 component mounted')
  },

  methods: {

    hello: function () {
      console.log('hello from Home2')
    }

  }

}
</script>

<style scoped></style>

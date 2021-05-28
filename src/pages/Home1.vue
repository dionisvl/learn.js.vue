<template>

  <div style="border:2px solid green; padding:15px">
    <div>
      <h3>Home1 component</h3>
      <div>
        <button v-on:click="emitExample">Run Home1 "Hello" method</button>
      </div>
    </div>

  </div>

</template>

<script>
export default {

  mounted() {
    console.log('Home1' + ' component mounted')
  },

  methods: {

    hello: function () {
      console.log('hello 1')
    },

    emitExample: function () {
      console.log('eventExampleEmit emit started in Home 1')
      this.$root.$emit('eventExampleEmit','arg1','arg2') //like this
    }

  }

}
</script>

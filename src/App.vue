<template>
  <div id="app">
    <hello-world :msg="'Hello World!'"></hello-world>
    <simple-form :my-array="myArray" />
  </div>
</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue"
import SimpleForm from "@/components/SimpleForm.vue"

export default {
  name: "VueApp",
  components: {
    HelloWorld,
    SimpleForm,
  },
  data: function () {
    return {
      myArray: ['dfghfxghbfgh','dfgbfdfgbxdfgb','sdffgdgdsfgh','dfgdfgdfgdfg'],
    }
  },
}
</script>

<style lang="scss">

</style>

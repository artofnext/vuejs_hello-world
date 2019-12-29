<template>
  <div id="app">
    <hello-world :msg="'Hello World!'"></hello-world>
  </div>
</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue"

export default {
  name: "Vue app",
  components: {
    HelloWorld,
  }
}
</script>

<style lang="scss">

</style>

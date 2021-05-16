<template>
  <figure class="figure">
    <Triangle />
  </figure>
</template>

<script lang="ts">
import { defineComponent } from "vue"
import Triangle from "./2021/05/15/Triangle.vue"

export default defineComponent({
  name: "App",
  components: {
    Triangle,
  },
})
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

<style lang="scss" scoped>
.figure {
  width: 500px;
  height: 400px;
  overflow: hidden;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>

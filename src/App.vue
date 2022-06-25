<template>
  <div class="container">
    <h1>Product</h1>
    <tablePage/>
  </div>
</template>

<script>
import tablePage from "@/view/TablePage.vue"
export default {
  name: "App",
  components:{
    tablePage
  }



}
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

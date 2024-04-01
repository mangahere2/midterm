<script>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import Navbar from './components/Navbar.vue'
export default{
  components: {Navbar}
}
</script>

<template>
  
  <div class="app">
    <Navbar />
    <RouterView />
  </div>
</template>

<style scoped>

</style>

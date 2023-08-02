<template>
  <Navbar/>
  <router-view/>
</template>

<script>
import Navbar from '@/components/Navbar.vue';

export default {
  name: 'App',
  components : {
      Navbar
  },
  components: {Navbar}
}
</script>

<style>
  #app {
      font-family: Arial, Helvetica, sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-os-font-smoothing: grayscale;
      color: rgb(0,0,0);
  }
</style>
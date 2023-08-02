<template>
    <center>
    <h1>Contact</h1>
</center>
  </template>
  <script>
  import { onMounted } from 'vue';
  export default {
      setup(props, context)
      {
          onMounted(() => {
              context.emit("id-menu", 2)
          })
      }
  }
  </script>
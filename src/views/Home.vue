<template>
  <center>
    <h1>Home Page</h1>
  </center>
    
  </template>
  <script>
  import { onMounted } from 'vue';
  
  export default {
    setup(props, context)
    {
        onMounted(() => {
            context.emit("id-menu", 1)
        })
    }
  }
  </script>
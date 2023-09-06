<template>
    <div class="home">
      <Home msg=" 123 teste msg"/>
    </div>
  </template>
  
  <script>
  // @ is an alias to /src
  import Home from '@/components/purchase'
//  import Home from '@/components/home'
  
  export default {
    name: 'HomeView',
    components: {
      Home
    }
  }
  </script>
  
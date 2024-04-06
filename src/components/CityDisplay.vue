<template>
    <div class="city-display">
      <p>Your city: {{ city }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'CityDisplay',
    props: {
      city: String
    }
  }
  </script>
  
  <style scoped>
  .city-display {
    /* CSS styles */
  }
  </style>
  
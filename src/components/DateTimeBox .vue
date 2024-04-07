<template>
    <div class="date-time-box">
      <p>{{ dateTime }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'DateTimeBox',
    props: {
      dateTime: String
    }
  }
  </script>
  
  <style scoped>
  .date-time-box {
    text-align: center;
    font-size: 24px;
  }
  
  </style>
  
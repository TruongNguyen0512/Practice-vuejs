<template>
    <div class="humidity-box">
      <p>{{ humidity }}</p>
      <p>Humidity</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'HumidityBox',
    props: {
      humidity: String
    }
  }
  </script>
  
  <style scoped>
  .humidity-box {
    text-align: center;
  }
  
  .humidity-box p:first-child {
    font-size: 24px; /* Điều chỉnh kích thước chữ tùy ý */
  }
  
  .humidity-box p:last-child {
    font-size: 16px; /* Điều chỉnh kích thước chữ tùy ý */
    color: #888; /* Màu chữ */
  }
  </style>
  
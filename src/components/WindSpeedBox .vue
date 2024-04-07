<template>
    <div class="wind-speed-box">
      <p>{{ windSpeed }}</p>
      <p>Wind Speed</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'WindSpeedBox',
    props: {
      windSpeed: String
    }
  }
  </script>
  
  <style scoped>
  .wind-speed-box {
    text-align: center;
  }
  
  .wind-speed-box p:first-child {
    font-size: 24px; /* Điều chỉnh kích thước chữ tùy ý */
  }
  
  .wind-speed-box p:last-child {
    font-size: 16px; /* Điều chỉnh kích thước chữ tùy ý */
    color: #888; /* Màu chữ */
  }
  </style>
  
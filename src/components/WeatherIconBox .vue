<template>
    <div class="weather-icon-box">
      <img :src="weatherIcon" alt="Weather Icon" class="weather-icon">
      <p class="temperature">{{ temperature }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'WeatherIconBox',
    props: {
      weatherIcon: String,
      temperature: String
    }
  }
  </script>
  
  <style scoped>
  .weather-icon-box {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  
  .weather-icon {
    width: 50px; /* Điều chỉnh kích thước tùy ý */
    height: auto;
  }
  
  .temperature {
    margin-top: 10px;
    font-size: 18px; /* Điều chỉnh kích thước chữ tùy ý */
  }
  </style>
  
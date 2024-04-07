<template>
  <div class="left-box">
    <div class="small-box">
      <DateTimeBox :dateTime="dateTime" />
    </div>
    <div class="small-box">
      <WeatherIconBox :weatherIcon="weatherIcon" :temperature="temperature" />
    </div>
    <div class="small-box">
      <HumidityBox :humidity="humidity" />
    </div>
    <div class="small-box">
      <WindSpeedBox :windSpeed="windSpeed" />
    </div>
  </div>
</template>

<script>
import DateTimeBox from './DateTimeBox .vue';
import WeatherIconBox from './WeatherIconBox .vue';
import HumidityBox from './HumidityBox .vue';
import WindSpeedBox from './WindSpeedBox .vue';
export default {
  name: 'LeftBox',
  props: {
    dateTime: String,
    weatherIcon: String,
    temperature: String,
    humidity: String,
    windSpeed: String
  },
  components: {
    DateTimeBox,
    WeatherIconBox,
    HumidityBox,
    WindSpeedBox
  }
}
</script>

<style scoped>
.left-box {
  display: flex;
  justify-content: space-around;
  align-items: center;
  width: 100%;
  height: 200px; /* Điều chỉnh chiều cao tùy ý */
  background-color: #f0f0f0;
  border: 1px solid #ccc;
}

.small-box {
  width: 23%; /* Điều chỉnh kích thước tùy ý */
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  border-right: 1px solid #ccc;
}

.small-box:last-child {
  border-right: none;
}
</style>

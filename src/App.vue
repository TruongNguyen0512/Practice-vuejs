<template>
  <div>
     <CityDisplay :city="currentCity" />
     <SearchBox @search = "handleSearch" />
     <LeftBox 
      :dateTime="currentDateTime"
      :weatherIcon="currentWeatherIcon"
      :temperature="currentTemperature"
      :humidity="currentHumidity"
      :windSpeed="currentWindSpeed"
    />
  </div>

</template>


<script>
import CityDisplay from './components/CityDisplay.vue';
import LeftBox from './components/LeftBox.vue';
import SearchBox from './components/SearchBox.vue';


export default {
  name : 'App' , 
  data() {
    return {
      currentCity : 'Sai Gon',
      currentDateTime: 'April 8, 2024 12:00 PM',
      currentWeatherIcon: 'path/to/weather/icon.png',
      currentTemperature: '25°C',
      currentHumidity: '65%',
      currentWindSpeed: '10 km/h'
    }
  } , 

  components : {
    CityDisplay , 
    SearchBox ,
    LeftBox  
  } , 
  methods : {
    handleSearch(city) {
      this.currentCity = city
    }
  }
}
</script>

<style>

</style>

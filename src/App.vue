<template>
  <div>
     <CityDisplay :city="currentCity" />
     <SearchBox @search = "handleSearch" />
  </div>

</template>


<script>
import CityDisplay from './components/CityDisplay.vue';
import SearchBox from './components/SearchBox.vue';


export default {
  name : 'App' , 
  data() {
    return {
      currentCity : 'Sai Gon'
    }
  } , 

  components : {
    CityDisplay , 
    SearchBox 
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

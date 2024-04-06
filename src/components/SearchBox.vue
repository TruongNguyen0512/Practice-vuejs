<template>
    <div class="search-box">
      <input type="text" v-model="searchQuery" placeholder="Enter your city">
      <button @click="search">Search</button>
    </div>
  </template>
  
  <script>
  export default {
    name: 'SearchBox',
    data() {
      return {
        searchQuery: ''
      }
    },
    methods: {
      search() {
        // Handle search functionality here
        this.$emit('search', this.searchQuery);
      }
    }
  }
  </script>
  
  <style scoped>
  .search-box {
    /* CSS styles */
  }
  </style>
  
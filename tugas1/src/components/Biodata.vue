<!-- src/components/Biodata.vue -->
<template>
    <div class="biodata">
      <h2>{{ name }}</h2>
      <p><strong>Age:</strong> {{ age }}</p>
      <p><strong>Location:</strong> {{ location }}</p>
      <p><strong>Profession:</strong> {{ profession }}</p>
      <p><strong>Hobies:</strong> {{ Hobies }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Biodata',
    props: {
      name: String,
      age: Number,
      location: String,
      profession: String,
      Hobies: String,
      SocialMedia: String
    }
  }
  </script>
  
  <style scoped>
  .biodata {
    font-family: Arial, sans-serif;
    border: 1px solid #ddd;
    padding: 1em;
    border-radius: 8px;
    max-width: 300px;
    margin: auto;
  }
  .biodata h2 {
    margin: 0;
    color: #ffffff;
  }
  </style>
  
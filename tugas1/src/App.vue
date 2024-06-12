<script setup>
import Biodata from './components/Biodata.vue'
</script>

<template>
  <div class="app-container">
    <div class="personal-photo-container">
      <img src="./assets/10.jpeg" class="personal-photo" alt="Personal Photo" />
    </div>
  
  <Biodata 
      name="Naufal Arief Faisal" 
      age="22" 
      location="Pekanbaru, Riau" 
      profession="Mahasiswa" 
      Hobies="Tenis Meja"
    />
  </div>
</template>

<style scoped>
.app-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 10vh;
  background: linear-gradient(135deg, #ffa4a4, #9bcdff, #d1e8ff);
  padding: 100px;
  box-sizing: border-box;
}


.personal-photo {
  height: 150px;
  width: 150px;
  border-radius: 50%;
  object-fit: cover;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.personal-photo:hover {
  transform: scale(1.5);
  box-shadow: 0 0 15px rgba(36, 38, 37, 0.7);
}

.biodata {
  background: #ffa0a0;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  text-align: center;
  max-width: 300px;
}

.biodata h2 {
  margin: 0;
  color: #ffffff;
  font-size: 24px;
}

.biodata p {
  margin: 10px 0;
  font-size: 16px;
  color: #000000;
}
</style>
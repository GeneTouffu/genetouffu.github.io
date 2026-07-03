<script setup lang="ts">
</script>

<template>
  <div class="construction-container">
    <div class="diagonal-stripes"></div>
    <div class="banner">
      <h1>⚠️ This Page is Under Construction ⚠️</h1>
    </div>
  </div>
</template>

<style scoped>
.construction-container {
  width: 100%;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  position: relative;
}

.diagonal-stripes {
  position: absolute;
  width: 100%;
  height: 100%;
  background: repeating-linear-gradient(
    45deg,
    #FFD700,
    #FFD700 20px,
    #000000 20px,
    #000000 40px
  );
  z-index: 1;
}

.banner {
  position: relative;
  z-index: 2;
  background-color: #FFD700;
  color: #000000;
  padding: 30px 10px;
  border: 8px solid #000000;
  border-radius: 8px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
  text-align: center;
  max-width: 90%;
}

.banner h1 {
  font-size: 2.5em;
  font-weight: bold;
  margin: 0;
  color: #000000;
  letter-spacing: 2px;
  font-family: 'Arial', 'Helvetica', sans-serif;
  white-space: nowrap;
}

@media (max-width: 768px) {
  .banner h1 {
    font-size: 2em;
  }

  .banner {
    padding: 30px 40px;
  }
}
</style>

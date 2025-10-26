<script setup lang="ts">
import logo from '#/open_sourcery.png'
</script>

<template>
  <div class="navbar">
    <div class="left">
      <img :src="logo" alt="Open Sourcery Logo" class="Navbar_Logo" />
      <h3>UMD OPEN SOURCERY</h3>
    </div>
    <div class="right">
      <a href="#">About Us</a>
      <a href="#">Projects</a>
      <a href="#">Sponsors</a>
      <a href="#">Join</a>
    </div>
  </div>
</template>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;

  background-color: #0f5079;
  border: 1px solid #004f7a;
  padding: 8px 40px;
  border-radius: 8px 8px 8px 8px;

  font-family: 'Inter', sans-serif;
  z-index: 1000;
}

.navbar .left {
  display: flex;
  align-items: center;
  gap: 10px;
}

.navbar .right {
  display: flex;
  gap: 24px;
  align-items: center;
  flex-direction: row;
}

.navbar h3 {
  color: white;
  font-weight: 700;
  font-size: 0.9rem;
  margin: 0;
}
.navbar a {
  color: white;
  text-decoration: none;
  font-size: 0.9rem;
  transition: opacity 0.2s ease;
  margin: 0;
}
.navbar a:hover {
  opacity: 0.7;
}

.Navbar_Logo {
  width: 32px;
  height: 32px;
  object-fit: contain;
}
</style>

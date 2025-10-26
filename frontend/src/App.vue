<script setup lang="ts">
import logo from '#/open_sourcery.png'
</script>

<template>
  <div class="page">
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
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&display=swap');

.page {
  display: flex;
  justify-content: center;
  width: 100%;
}

.navbar {
  width: calc(1308 / 1440 * 100vw); /* 1308/1440 of the viewport width */
  display: flex;
  justify-content: space-between;
  align-items: center;

  background-color: rgba(15, 80, 121, 79);
  border: 0.0625rem solid #004f7a;
  padding: 0.5rem 2.5rem;
  border-radius: 0.5rem;

  font-family: 'Inter';
  z-index: 500;
  font-size: 1.5rem;
}

.navbar .left {
  display: flex;
  align-items: center;
  gap: 0.625rem;
  font-weight: 600;
}

.navbar .right {
  display: flex;
  gap: 1.5rem;
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
  width: 4.875rem;
  height: 4.875rem;
  object-fit: contain;
}
</style>

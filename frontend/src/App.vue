<script setup lang="ts">
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'
import AboutUs from '@/components/AboutUs.vue'
</script>

<template>
  <div class="page">
    <Navbar></Navbar>
    <AboutUs></AboutUs>
    <Footer></Footer>
  </div>
</template>

<style scoped>
.page {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.page > *:not(:last-child) {
  flex-shrink: 0;
}

/* Let AboutUs grow and push Footer down */
.page > .content {
  flex: 1;
}

</style>
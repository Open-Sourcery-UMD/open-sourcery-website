<script setup lang="ts">
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'
import AboutUs from '@/components/AboutUs.vue'
import Projects from '@/components/Projects.vue'
</script>

<template>
  <div class="page">
    <Navbar />
    <AboutUs title="About Us" />
    <Projects title="Projects" />
    <Footer />
  </div>
</template>

<style scoped>
.page {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  align-items: center;
}

.page > *:not(:last-child) {
  flex-shrink: 0;
}

/* Let AboutUs grow and push Footer down */
.page > .content {
  flex: 1;
}

</style>
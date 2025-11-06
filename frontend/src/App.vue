<script setup lang="ts">
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'
import SectionTitle from '@/components/SectionTitle.vue'
</script>

<template>
  <div class="page">
    <Navbar></Navbar>
    <SectionTitle title="About Us"></SectionTitle>
    <Footer></Footer>
  </div>
</template>

<style scoped>
.page {
  display: flex;
  align-items: center;
  flex-direction: column;
  min-height: 100vh;
  align-items: center;
}
</style>
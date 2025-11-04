<script setup lang="ts">
import { defineProps } from 'vue'

const { title } = defineProps<{ title: string }>()
</script>

<template>
    <div class="section_title">
        <h2>{{ title }}</h2>
        <div class="underline"></div>
    </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inria+Sans:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap');

.section_title {
  display: flex;
  flex-direction: column;
  align-items: center; /* centers children horizontally */
  margin: 3rem 0 2rem 0;
  text-align: center;
  font-family: "Inria Sans", sans-serif;
  opacity: 1;
}

.section_title h2 {
  font-size: 6rem;
  font-weight: 400;
  margin: 0;
  color: #1369A0;
}

.underline {
  width: 447px;
  height: 10px;
  background-color: #1369A0;
  margin-top: 0.5rem;
  border-radius: 10px;
}
</style>
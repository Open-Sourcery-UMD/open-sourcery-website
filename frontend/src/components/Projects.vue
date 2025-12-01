<script setup lang="ts">
import SectionTitle from '@/components/SectionTitle.vue'
import logo from '#/open_sourcery.png'
import Hexagon from './Hexagon.vue';
</script>

<template>
    <!-- Pass the background image to CSS using a variable -->
    <div class="page" :style="{ '--bg-image': `url(${logo})` }">
        <SectionTitle title="Projects" />

        <div class="projects-content">
            <Hexagon :width="384" :height="420" :image="logo" border-color="#000000"/>
            <Hexagon :width="465" :height="508" :image="logo" />
            <Hexagon :width="384" :height="420" :image="logo" />
        </div>
    </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inria+Sans:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap');

.page {
    position: relative;
    background-size: cover;
    background-position: center;
    display: flex;
    flex-direction: column;
    margin: 0 auto;
    height: 90rem;
    overflow: hidden; /* Prevent pseudo-element from spilling out */
}

/* Pseudo-element background with opacity */
.page::before {
    content: "";
    position: absolute;
    inset: 0;
    background-image: var(--bg-image);
    background-size: cover;
    background-position: center;
    opacity: 0.21; /* <<< adjust background opacity here */
    z-index: -1;
}

.projects-content {
    margin-top: 2rem;
    font-size: 1.2rem;
    line-height: 1.6;
    color: #055665;
    font-family: 'Inria Sans';
    font-weight: 500;
    display: flex;
    justify-content: center;
    gap: 2rem;
    align-items: center;
}
</style>

<script setup lang="ts">
import SectionTitle from '@/components/SectionTitle.vue'
</script>

<template>
    <div class="page">
        <SectionTitle title="About Us" />

        <div class="about-us-content">
            <p>
                Open Sourcery is a club for students interested in collaborative software development,
                especially open-source development, at the University of Maryland. Our goal is to provide
                a space for both experienced developers and newcomers to improve their coding and project
                management skills, acquire technical and open source experience through hands-on projects,
                and foster connections with fellow students with an interest in open-source software.
                Our focus is on project matchups and mentorship, as well as furthering the interest of
                open-source development on campus.
            </p>
        </div>
    </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Jura:wght@300..700&display=swap');

.page {
    display: flex;
    flex-direction: column;
    margin: 0 auto;        /* Horizontally center the entire page box */
    height: 90rem;
    width: 58.25rem;
}

.about-us-content {
    max-width: 1514.4rem;
    margin-top: 2rem;      /* Space below SectionTitle */
    font-size: 1.2rem;
    line-height: 1.6;
    color: #055665;
    font-family: 'Jura';
    font-weight: 500;
}
</style>

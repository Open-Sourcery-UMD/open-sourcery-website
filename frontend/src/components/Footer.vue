<script setup lang="ts">

import logo from '#/open_sourcery.png'
import discord from '#/Discord_Image.png'
import github from '#/Github_Image.png'
import instagram from '#/Instagram_Image.png'
import mail from '#/Mail_Image.png'

const props = defineProps<{
  title?: string
}>()

const socials = [
  {
    name: 'GitHub',
    src: github,
    href: 'https://github.com/Open-Sourcery-UMD',
    class: 'Footer_GH_Logo'
  },
  {
    name: 'Instagram',
    src: instagram,
    href: 'https://www.instagram.com/umdopensourcery/',
    class: 'Footer_IG_Logo'
  },
  {
    name: 'Discord',
    src: discord,
    href: 'https://discord.com/invite/BWvbpgskZT',
    class: 'Footer_DISCORD_Logo'
  },
  {
    name: 'Email',
    src: mail,
    href: 'mailto:umdopensourcery@gmail.com',
    class: 'Footer_EMAIL_Logo'
  }
]
</script>

<template>
  <footer class="footer">
    <img :src="logo" alt="Open Sourcery Logo" class="Footer_Logo" />

    <h3 v-html="(title ?? 'OPEN<br>SOURCERY')"></h3>

    <div class="socials">
      <a v-for="(s, i) in socials" :key="i" :href="s.href" target="_blank" rel="noopener noreferrer">
        <img :src="s.src" :alt="`${s.name} Logo`" :class="s.class" />
      </a>
    </div>
  </footer>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=K2D&display=swap');

.footer {
  position: relative;
  min-height: 20.125rem;
  /* if you need that Figma height */
  padding: 2rem 3rem;
}

.footer {
  width: 100%;
  height: 20.125rem;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  gap: 1rem;
  font-family: 'K2D';
  padding: 2rem 3rem;
  background-color: #075180;
  box-sizing: border-box;
}

.socials {
  margin-left: auto;
  /* pushes to the right */
  display: flex;
  align-items: center;
  gap: 2rem;
}

.footer h3 {
  font-size: 4rem;
  font-weight: 400;
  color: white;
}

.Footer_Logo {
  width: 16.5rem;
  height: auto;
  object-fit: contain;
}

.Footer_GH_Logo {
  width: 6.188rem;
  height: auto;
  object-fit: contain;
}

.Footer_IG_Logo {
  width: 4.438rem;
  height: auto;
  object-fit: contain;
}

.Footer_DISCORD_Logo {
  width: 5.875rem;
  height: auto;
  object-fit: contain;
}

.Footer_EMAIL_Logo {
  width: 5.625rem;
  height: auto;
  object-fit: contain;
}
</style>
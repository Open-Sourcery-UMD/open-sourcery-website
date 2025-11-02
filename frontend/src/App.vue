<script setup lang="ts">
import logo from '#/open_sourcery.png'
import discord from '#/Discord_Image.png'
import github from '#/Github_Image.png'
import instagram from '#/Instagram_Image.png'
import mail from '#/Mail_Image.png'
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

    <div class="footer">
      <img :src="logo" alt="Open Sourcery Logo" class="Footer_Logo" />
      <h3>OPEN<br>SOURCERY</h3>

      <div class="socials">
        <a href="https://github.com/Open-Sourcery-UMD"><img :src="github" alt="Github Logo"
            class="Footer_GH_Logo" /></a>
        <a href="https://www.instagram.com/umdopensourcery/"><img :src="instagram" alt="Instagram Logo"
            class="Footer_IG_Logo" /></a>
        <a href="https://discord.com/invite/BWvbpgskZT"><img :src="discord" alt="Discord Logo"
            class="Footer_DISCORD_Logo" /></a>
        <a href="mailto:umdopensourcery@gmail.com"><img :src="mail" alt="Email" class="Footer_EMAIL_Logo" /></a>
      </div>
    </div>

  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&family=K2D&display=swap');

.page {
  display: flex;
  justify-content: center;
  width: 100%;
}

.navbar {
  width: calc(1308 / 1440 * 100vw);
  /* 1308/1440 of the viewport width */
  height: 5.313rem;
  display: flex;
  justify-content: space-between;
  align-items: center;

  background-color: rgba(15, 80, 121, 0.79);
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
  font-weight: 600;
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


.footer {
  position: relative;
  min-height: 20.125rem;
  /* if you need that Figma height */
  padding: 2rem 3rem;
}

.footer {
  position: absolute;
  /* Stay at the bottom of the screen */
  bottom: 0;
  /* Place it at the bottom */
  left: 0;
  /* Align it with the left edge */
  width: 100%;
  /* Full width of the screen */
  height: 20.125rem;
  /* Fixed height */
  display: flex;
  /* Flexbox to position children */
  align-items: center;
  /* Vertically center content */
  gap: 1rem;
  /* Space between items */
  justify-content: flex-start;
  /* Align content to the left */
  font-family: 'K2D';
  /* Custom font */
  padding: 2rem 3rem;
  /* Padding */
  background-color: #075180;
  /* Footer background color */
  box-sizing: border-box;
  /* Include padding in width calculation */
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
  width: 6.188rem;
  height: auto;
  object-fit: contain;
}

.Footer_DISCORD_Logo {
  width: 6.188rem;
  height: auto;
  object-fit: contain;
}

.Footer_EMAIL_Logo {
  width: 6.188rem;
  height: auto;
  object-fit: contain;
}
</style>
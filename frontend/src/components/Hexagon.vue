<script setup lang="ts">
defineProps({
  width: { type: Number, default: 200 },
  height: { type: Number, default: 200 },
  borderSize: { type: Number, default: 2 },
  borderColor: { type: String, default: "#000000" },
  image: { type: String, required: true },
})
</script>

<template>
  <svg
    :width="width"
    :height="height"
    viewBox="0 0 100 100"
    class="hex"
  >
    <!-- Border hexagon -->
    <polygon
      :stroke="borderColor"
      :stroke-width="borderSize"
      fill="none"
      points="50 0, 93 25, 93 75, 50 100, 7 75, 7 25"
    />

    <!-- Image masked to hex shape -->
    <defs>
      <clipPath id="hexMask">
        <polygon points="50 0, 93 25, 93 75, 50 100, 7 75, 7 25" />
      </clipPath>
    </defs>

    <image
      :href="image"
      x="0"
      y="0"
      width="100"
      height="100"
      preserveAspectRatio="xMidYMid slice"
      clip-path="url(#hexMask)"
    />
  </svg>
</template>

<style scoped>
.hex {
  display: block;
}
</style>

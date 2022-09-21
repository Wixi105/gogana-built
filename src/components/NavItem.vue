<template>
  <div class="flex my-5">
    <svg
      xmlns="http://www.w3.org/2000/svg"
      fill="none"
      viewBox="0 0 24 24"
      stroke-width="1.5"
      stroke="currentColor"
      class="w-5 mr-4"
    >
      {{ svgPath }}
    </svg>
    <p>{{ itemLabel }}</p>
  </div>
</template>

<script setup>
defineProps(["svgPath", "itemLabel"]);
</script>

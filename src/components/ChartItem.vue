<template>
  <div
    class="py-7 px-5 border border-gray-500 border-opacity-30 w-1/3 rounded-lg"
  >
    <section>
      <p class="text-sm">{{ label }}</p>
      <p class="text-2xl font-bold">{{ price }}</p>
      <p class="text-sm text-gray-500">{{ desc }}</p>
    </section>
  </div>
</template>

<script setup>
defineProps(["label", "price", "desc"]);
</script>

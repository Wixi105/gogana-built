<template>
  <div
    class="py-7 px-5 border border-gray-500 border-opacity-20 w-1/3 rounded-lg"
  >
    <section>
      <p class="text-xs pb-1">{{ label }}</p>
      <p class="text-2xl font-bold">{{ price }}</p>
      <p class="text-xs text-gray-500 pt-1">{{ desc }}</p>
    </section>
    <section>
      <div class="border-2 rounded-full"></div>
    </section>
  </div>
</template>

<script setup>
defineProps(["label", "price", "desc"]);
</script>

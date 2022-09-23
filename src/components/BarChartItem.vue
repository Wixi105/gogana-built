<template>
  <div
    class="p-5 border border-gray-500 border-opacity-20 rounded-lg flex justify-between"
  >
    <div>
      <p class="font-medium mb-3">Total Revenue</p>
      <section class="flex items-center text-xs">
        <p class="text-2xl font-semibold">$50.4K</p>
        <p class="text-green-600 ml-3 flex items-center">
          8% than last month
          <span
            ><svg
              class="w-3 ml-2"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 10l7-7m0 0l7 7m-7-7v18"
              ></path></svg
          ></span>
        </p>
      </section>
    </div>
    <div class="flex items-center">
      <p class="text-xs mr-4">Data updates every 3 hours</p>
      <button class="text-black bg-gray-100 py-2 px-4 text-xs rounded-sm">
        View All Orders
      </button>
    </div>
  </div>
</template>

<script setup></script>

<template>
  <div class="flex">
    <div class="w-1/5">
      <SideBar />
    </div>
    <!-- Header -->
    <div class="w-4/5 p-10 mt-4 flex justify-between h-fit items-center">
      <p class="text-xl font-medium">Dashboard</p>

      <div class="flex items-center">
        <section class="relative">
          <input
            type="text"
            placeholder="Search Here..."
            class="bg-gray-100 placeholder:font-light placeholder:text-start pl-10 text-sm border-none rounded-full w-[400px] py-3 px-2 focus:border-n-secondary-20 focus:outline focus:outline-1 focus:outline-n-secondary-20"
          />
          <svg
            class="absolute top-[13px] left-4 h-5 pointer-events-none"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
            ></path>
          </svg>
        </section>
        <!-- Bell Start -->
        <section class="border border-gray-300 p-2 rounded-full h-fit ml-8">
          <svg
            class="w-5"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9"
            ></path>
          </svg>
        </section>
        <!-- Bell End -->
        <section class="ml-8">
          <div>
            <p class="text-sm font-semibold">Alex Mora</p>
            <p class="text-xs font-regular">Super Admin</p>
          </div>
        </section>
      </div>
    </div>
    <!-- Header End -->
  </div>
</template>

<script setup>
import SideBar from "./views/SideBar.vue";
</script>

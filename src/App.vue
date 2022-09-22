<template>
  <div class="flex">
    <div class="w-1/5">
      <SideBar />
    </div>
    <!-- Right Side -->
    <div class="w-4/5 p-10 mt-4 h-fit">
      <div class="flex justify-between items-center">
        <!-- Header Start -->
        <p class="text-xl font-medium">Dashboard</p>

        <div class="flex items-center">
          <section class="relative">
            <input
              type="text"
              placeholder="Search Here..."
              class="bg-gray-100 placeholder:font-light placeholder:text-start pl-10 text-sm border-none rounded-full w-[400px] py-3 px-2 transition-all duration-500 focus:border-n-secondary-20 focus:outline focus:outline-1 focus:outline-gray-300"
            />
            <svg
              class="absolute top-[13px] left-4 h-5 pointer-events-none"
              fill="none"
              stroke="#9e9e9e"
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
          <section
            class="border border-gray-300 p-2 rounded-full h-fit ml-10 relative cursor-pointer"
          >
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
            <!-- Bell Dot Icon SVG -->
            <svg
              class="absolute top-1 left-3"
              width="20px"
              height="20px"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <circle
                cx="12"
                cy="12"
                r="4"
                fill="#FF7F50"
                fill-rule="evenodd"
              />
            </svg>
            <!-- Bell Dot Icon SVG End -->
          </section>
          <!-- Bell End -->
          <!-- Profile Start -->
          <section class="ml-10 flex items-center">
            <div>
              <p class="text-sm font-semibold">Alex Mora</p>
              <p class="text-xs font-regular">Super Admin</p>
            </div>
            <img
              class="w-12 h-12 rounded-full object-cover ml-3"
              src="https://images.pexels.com/photos/1681010/pexels-photo-1681010.jpeg?auto=compress&cs=tinysrgb&w=1200"
              alt=""
            />
          </section>
          <!-- Profile End -->
        </div>
        <!-- Header End -->
      </div>
      <!-- Chart Item Start -->
      <div class="flex justify-around mt-16">
        <ChartItem
          label="Today's Sales"
          price="$20.4K"
          desc="We have sold 123 items"
        />
        <ChartItem
        class="ml-5"
          label="Today's Revenue"
          price="$8.2K"
          desc="Available to Payout"
        />
        <ChartItem
        class="ml-5"
          label="In Escrow"
          price="$18.2K"
          desc="Available to payout"
        />
      </div>
      <!-- Chart Item End -->
    </div>
    <!-- Right Side End -->
  </div>
</template>

<script setup>
import SideBar from "./views/SideBar.vue";
import ChartItem from "./components/ChartItem.vue";
</script>

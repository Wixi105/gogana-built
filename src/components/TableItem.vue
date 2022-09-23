<template>
  <div class="border border-gray-500 border-opacity-20 rounded-lg">
    <section class="flex justify-between p-5 items-center">
      <p class="text-sm font-medium">Latest Orders</p>
      <div class="flex items-center">
        <p class="text-xs text-gray-400">Data Updates Every 3 Hours</p>
        <button
          class="px-3 py-2 bg-blue-600 text-xs text-white rounded-md ml-5"
        >
          View All Orders
        </button>
      </div>
    </section>
    <section class="bg-gray-100">
      <ul class="grid grid-cols-9 gap-6 mt-2 px-5 py-2 text-sm">
        <li class="col-span-2">Products</li>
        <li class="place-self-center">Order ID</li>
        <li class="place-self-center">Date</li>
        <li class="place-self-center col-span-2">Customer name</li>
        <li class="place-self-center">Status</li>
        <li class="place-self-center">Amount</li>
        <li class="place-self-end">Action</li>
      </ul>
    </section>
    <section>
      <ul
        class="grid grid-cols-9 gap-6 mt-2 px-5 py-2 text-sm mb-4"
        v-for="datum in data"
        :key="datum.order_id"
      >
        <li class="place-self-start flex col-span-2">
          <div class="w-12">
            <img
              :src="datum.product_image"
              alt="Product image"
              class="object-cover w-12 rounded-md"
            />
          </div>
          <p class="ml-4 self-center">{{ datum.product_name }}</p>
        </li>
        <li class="justify-self-center self-center">{{ datum.order_id }}</li>
        <li class="justify-self-center self-center">{{ datum.date }}</li>
        <li class="justify-self-center col-span-2 self-center">
          {{ datum.name }}
        </li>
        <li
          class="justify-self-center text-sm self-center px-4 py-1 rounded-md"
          :class="
            datum.status === 'Pending'
              ? 'text-yellow-700 bg-yellow-100 border border-yellow-300'
              : 'text-green-700 bg-green-100 border border-green-300'
          "
        >
          {{ datum.status }}
        </li>
        <li class="justify-self-center self-center">{{ datum.amount }}</li>
        <li class="justify-self-end">
          <svg
            class="w-6 h-6 self-center"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M5 12h.01M12 12h.01M19 12h.01M6 12a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0z"
            ></path>
          </svg>
        </li>
      </ul>
    </section>
  </div>
</template>

<script setup>
import { ref } from "vue";

const data = ref([
  {
    product_image:
      "https://images.pexels.com/photos/4841324/pexels-photo-4841324.jpeg?auto=compress&cs=tinysrgb&w=1200",
    product_name: "Oranges",
    order_id: "11232",
    date: "Jun 29, 2022",
    name: "Anastasia Hasuna",
    status: "Delivered",
    amount: "$1100.00",
  },
  {
    product_image:
      "https://images.pexels.com/photos/607812/pexels-photo-607812.jpeg?auto=compress&cs=tinysrgb&w=1200",
    product_name: "iPhone 13",
    order_id: "11233",
    date: "Jun 23, 2022",
    name: "John Wick",
    status: "Pending",
    amount: "$5100.00",
  },
  {
    product_image:
      "https://images.pexels.com/photos/1767434/pexels-photo-1767434.jpeg?auto=compress&cs=tinysrgb&w=1200",
    product_name: "Love",
    order_id: "11234",
    date: "Apr 30, 2022",
    name: "Anastasia Hasuna",
    status: "Delivered",
    amount: "$1100.00",
  },
  {
    product_image:
      "https://images.pexels.com/photos/1229861/pexels-photo-1229861.jpeg?auto=compress&cs=tinysrgb&w=1200",
    product_name: "MacBook Pro 2016",
    order_id: "11235",
    date: "Mar 1, 2021",
    name: "Endeavor Asante",
    status: "Pending",
    amount: "$9000.00",
  },
  {
    product_image:
      "https://images.pexels.com/photos/2762247/pexels-photo-2762247.jpeg?auto=compress&cs=tinysrgb&w=1200",
    product_name: "Black Chair",
    order_id: "11236",
    date: "Jun 7, 2022",
    name: "Bruno Fernandes",
    status: "Delivered",
    amount: "$6100.00",
  },
  {
    product_image:
      "https://images.pexels.com/photos/47730/the-ball-stadion-football-the-pitch-47730.jpeg?auto=compress&cs=tinysrgb&w=1200",
    product_name: "Harry Maguire",
    order_id: "11237",
    date: "Jun 29, 2022",
    name: "Chelsea Football Club",
    status: "Pending",
    amount: "Free",
  },
  {
    product_image:
      "https://images.pexels.com/photos/324557/pexels-photo-324557.jpeg?auto=compress&cs=tinysrgb&w=1200",
    product_name: "Simpons Coke Can",
    order_id: "11238",
    date: "Feb 2, 2022",
    name: "Aisha Huang",
    status: "Delivered",
    amount: "$109100.00",
  },
]);
</script>

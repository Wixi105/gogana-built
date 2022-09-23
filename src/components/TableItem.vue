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
      <ul class="flex justify-between mt-2 px-5 py-2 text-sm">
        <li>Products</li>
        <li>Order ID</li>
        <li>Date</li>
        <li>Customer name</li>
        <li>Status</li>
        <li>Amount</li>
        <li>Action</li>
      </ul>
    </section>
    <section>
      <ul class="flex justify-between mt-2 px-5 py-2">
        <li>Products</li>
        <li>Order ID</li>
        <li>Date</li>
        <li>Customer name</li>
        <li>Status</li>
        <li>Amount</li>
        <li>Action</li>
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
    action: "url",
  },
  {
    product_image:
      "https://images.pexels.com/photos/607812/pexels-photo-607812.jpeg?auto=compress&cs=tinysrgb&w=1200",
    product_name: "iPhone 13",
    order_id: "11233",
    date: "Jun 23, 2022",
    name: "John Wick",
    status: "Not Delivered",
    amount: "$5100.00",
    action: "url",
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
    action: "url",
  },
  {
    product_image:
      "https://images.pexels.com/photos/1229861/pexels-photo-1229861.jpeg?auto=compress&cs=tinysrgb&w=1200",
    product_name: "MacBook Pro 2016",
    order_id: "11235",
    date: "Mar 1, 2021",
    name: "Endeavor Asante",
    status: "Not Delivered",
    amount: "$9000.00",
    action: "url",
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
    action: "url",
  },
  {
    product_image:
      "https://images.pexels.com/photos/47730/the-ball-stadion-football-the-pitch-47730.jpeg?auto=compress&cs=tinysrgb&w=1200",
    product_name: "Harry Maguire",
    order_id: "11237",
    date: "Jun 29, 2022",
    name: "Anastasia Hasuna",
    status: "Not Delivered",
    amount: "Free",
    action: "url",
  },
  {
    product_image:
      "https://images.pexels.com/photos/1009158/pexels-photo-1009158.jpeg?auto=compress&cs=tinysrgb&w=1200",
    product_name: "Simpons Coke Can",
    order_id: "11238",
    date: "Feb 2, 2022",
    name: "Aisha Huang",
    status: "Delivered",
    amount: "$109100.00",
    action: "url",
  },
]);
</script>

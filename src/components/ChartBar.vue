<template>
  <BarChart
    :chart-data="data"
    :options="options"
    css-classes="chart-container"
  />
</template>

<script setup>
import { BarChart } from "vue-chart-3";
import { ref, computed } from "vue";

import {
  Chart,
  BarController,
  CategoryScale,
  LinearScale,
  BarElement,
} from "chart.js";

Chart.register(BarController, CategoryScale, LinearScale, BarElement);

const dataValues = ref([
  [1, 3, 5, 7, 2, 4, 6],
  [1, 5, 2, 6, 3, 7, 4],
]);

const data = computed(() => ({
  labels: ["Jan", "Feb", "Mar", "April", "May", "Jun", "Jul", "Aug", "Sep"],
  datasets: [
    {
      label: "Foo",
      data: dataValues.value[0],
      backgroundColor: "#FEFEFE",
    },
    {
      label: "Bar",
      data: dataValues.value[1],
      backgroundColor: "#2369C4",
    },
  ],
}));

const options = ref({
  plugins: {
    title: {
      text: "Bar",
    },
  },
});
</script>

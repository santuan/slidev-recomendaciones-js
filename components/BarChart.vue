<template>
  <Bar :data="data" :options="options" />
</template>

<script lang="ts">
import {
  Chart as ChartJS,
  Title,
  Tooltip,
  Legend,
  BarElement,
  CategoryScale,
  LinearScale
} from 'chart.js'
import { Bar } from 'vue-chartjs'

ChartJS.register(CategoryScale, LinearScale, BarElement, Title, Tooltip, Legend)

export default {
  name: 'App',
  components: {
    Bar
  },
  data() {
    return {
      data: {
        labels: ['Frontend', 'Backend', 'Mobile', 'Desktop', 'Data visualization', 'Graphics & Animation', 'Data Analysis', 'Game Development', 'Embedded Apps', 'Machine Learning'],
        datasets: [
          {
            backgroundColor: [
              "#845EC2",
              "#9164B9",
              "#9F6AB0",
              "#AD70A7",
              "#BA769E",
              "#C87D95",
              "#D6838C",
              "#E38983",
              "#F18F7A",
              "#FE613F",
              "#FE613F",
              "#FE613F",
            ],
            data: [29805, 19769, 8186, 6096, 5484, 4013, 2477, 1766, 907, 661],
          },
        ],

      },
      options: {
        indexAxis: 'y',
        maintainAspectRatio: false,
        // Elements options apply to all of the options unless overridden in a dataset
        // In this case, we are setting the border of each horizontal bar to be 2px wide
        responsive: true,
        plugins: {
          legend: {
            display: false
          },
          title: {
            display: true,
            text: 'Para que se utiliza Javascript (2022.stateofjs.com)'
          }
        }
      },
    }
  }
}
</script>
<template>
    <Doughnut
      id="my-chart-id"
      :options="chartOptions"
      :data="chartData"
    />
  </template>
  
  <script>
  import { Doughnut } from 'vue-chartjs'
  import { Chart as ChartJS, ArcElement, Tooltip, Legend } from 'chart.js'
  
  ChartJS.register(ArcElement, Tooltip, Legend)
  
  export default {
    name: 'App',
    components: { Doughnut },
    data() {
      return {
        chartData: {
          labels: [ 'January', 'February', 'March' ],
          datasets: [ {
            backgroundColor: ['#41B883', '#E46651', '#00D8FF', '#DD1B16'],
            data: [40, 20, 12] 
        } ]
        },
        chartOptions: {
          responsive: true
        }
      }
    }
  }
  </script>
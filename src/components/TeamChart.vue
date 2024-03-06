<script>
import { Bar } from "vue-chartjs";
import {
  Chart as ChartJS,
  Title,
  Tooltip,
  Legend,
  BarElement,
  CategoryScale,
  LinearScale,
} from "chart.js";
import teamChartData from "../team-data.js";
import planetChartData from "../team-data.js";
ChartJS.register(
  Title,
  Tooltip,
  Legend,
  BarElement,
  CategoryScale,
  LinearScale
);
//const ctx = document.getElementById("team-chart");
//const myChart = new Chart(ctx, teamChartData);

export default {
  name: "TeamChart",
  components: { Bar },
  data() {
    return {
      chartData: {
        labels: ["Wins", "Losses"],
        datasets: [
          {
            data: [130, 71],
          },
        ],
      },
      chartOptions: {
        responsive: true,
      },
    };
  },
};
</script>

<template>
  <div class="team-graph">
    <Bar id="team-chart" :options="chartOptions" :data="chartData" />
  </div>
</template>

<style>
.team-graph {
  background-color: aqua;
  width: 60%;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>

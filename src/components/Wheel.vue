<script>
import { Pie } from 'vue-chartjs'

export default {
  extends: Pie,
  data: () => ({
    chartdata: {
      labels: ['1', '5', '10', '50'],
      datasets: [
        {
          data: [1, 2, 3, 4],
          backgroundColor: [
            'rgba(255, 100, 130, 0.2)',
            'rgba(100, 130, 255, 0.2)',
            'rgba(130, 255, 100, 0.2)',
            'rgba(230, 210, 85, 0.2)'
          ]
        }
      ]
    },
    options: {
      responsive: true,
      legend: {
        display: false
      }
    }
  }),

  mounted () {
    this.renderChart(this.chartdata, this.options)
  }
}
</script>


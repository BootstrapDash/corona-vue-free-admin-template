<script lang='js'>
import {
  Doughnut
} from 'vue-chartjs'
export default {
  extends: Doughnut,
  props: {
    labels: {
      type: Array,
      default: () => ["Paypal", "Stripe","Cash"]
    },
  },
  data () {
    return {
      gradient: null,
      gradient2: null
    }
  },
  mounted () {
    this.renderChart({
      labels: this.labels,
      datasets: [{
        labels: ["Paypal", "Stripe","Cash"],
        data: [55, 25, 20],
        backgroundColor: [
              "#111111","#00d25b","#ffab00"
            ],
        borderWidth: 0
      }]
    }, {
      responsive: true,
      cutoutPercentage: 70,
      animation: {
        animateScale: true,
        animateRotate: true
      },
      legend: false
    })
  }
}
</script>

<style scoped lang='scss'>
  .transactionHistory {

  }
</style>

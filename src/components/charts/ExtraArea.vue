<template>

    <area-chart
        id="area"
        :data="areaData"
        xkey="period"
        ykeys='[ "iphone", "imac", "samsung", "nokia", "xiaomi" ]'
        resize="true"
        labels='[ "iPhone", "iMac", "iMac", "iMac", "iMac" ]'

        line-colors= '[ "#26DAD2", "#fc6180", "#62d1f3", "#ffb64d", "#4680ff" ]'


        grid="false"
        grid-text-weight="bold"
        hide-hover="auto"

        point-size= 0
        line-width= 0
        fill-opacity= 0.8
        behave-like-line= "true"
        grid-line-color= "#e0e0e0"
    >
    </area-chart>

</template>

<script>
// Do not forget to import raphael
import Raphael from 'raphael/raphael'
import jquery from 'jquery'
global.Raphael = Raphael

import Vue from 'vue'
import { AreaChart } from 'vue-morris'

export default {
    //extends: AreaChart,
    //name: 'morris-chart',
    data() {
        return{
            // donutData: [
            //     { label: 'Red', value: 300 },
            //     { label: 'Blue', value: 50 },
            //     { label: 'Yellow', value: 100 }
            // ]
          areaData: [
                  {
                    period: '2001',
                    iphone: 0,
                    imac: 0,
                    ibook: 90,
                    samsung: 0,
                    android: 0
                }, {
                    period: '2002',
                    iphone: 10,
                    imac: 60,
                    ibook: 40,
                    samsung: 80,
                    android: 120
                }, {
                    period: '2003',
                    iphone: 120,
                    imac: 10,
                    ibook: 90,
                    samsung: 30,
                    android: 50
                }, {
                    period: '2004',
                    iphone: 0,
                    imac: 0,
                    ibook: 120,
                    samsung: 0,
                    android: 0
                }, {
                    period: '2005',
                    iphone: 0,
                    imac: 0,
                    ibook: 0,
                    samsung: 150,
                    android: 0
                }, {
                    period: '2006',
                    iphone: 160,
                    imac: 75,
                    ibook: 30,
                    samsung: 60,
                    android: 90
                }, {
                    period: '2007',
                    iphone: 10,
                    imac: 120,
                    ibook: 40,
                    samsung: 60,
                    android: 30
                }
              ]
        }

    },
    components: {
        AreaChart
    }

}



// import { Line } from 'vue-chartjs';

// export default {
//    extends: Line,
//    data() {
//       return {
//          datacollection: {
//             //Data to be represented on x-axis
//             labels: ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December'],
//             datasets: [{
//                label: 'Data One',
//                backgroundColor: '#f87979',
//                pointBackgroundColor: 'white',
//                borderWidth: 1,
//                pointBorderColor: '#249EBF',
//                //Data to be represented on y-axis
//                data: [40, 20, 30, 50, 90, 10, 20, 40, 50, 70, 90, 100]
//             }]
//          },
//          //Chart.js options that controls the appearance of the chart
//          options: {
//             scales: {
//                yAxes: [{
//                   ticks: {
//                      beginAtZero: true
//                   },
//                   gridLines: {
//                      display: true
//                   }
//                }],
//                xAxes: [{
//                   gridLines: {
//                      display: false
//                   }
//                }]
//             },
//             legend: {
//                display: true
//             },
//             responsive: true,
//             maintainAspectRatio: false
//          }
//       }
//    },
//    mounted() {
//       //renderChart function renders the chart with the datacollection and options object.
//       this.renderChart(this.datacollection, this.options)
//    }
// }
</script>


<style>

</style>
<template>
<q-card class="q-mt-md" style="height:392px;margin-top:15px">
    <div class="text-subtitle2 q-pa-md">Different Types of Sources</div>
  <apexcharts
  style="margin-top:20px"
    height="280px"
    type="donut"
    :options="plotOptions"
    :series="series"
  ></apexcharts>
</q-card>
</template>

<script>
import VueApexCharts from "vue-apexcharts";

export default {
  name: "PieChart",
  components: {
    apexcharts: VueApexCharts
  },
  data: function() {
    return {
      plotOptions: {
        colors: ['#ff9999', '#21BA45', '#9C27B0', '#E91E63', '#F2C037'],
        pie: {
            startAngle: 0,
            endAngle: 360,
            expandOnClick: true,
            offsetX: 0,
            offsetY: 0,
            customScale: 1,
            dataLabels: {
                offset: 0,
                minAngleToShowLabel: 10
            }, 
        donut: {
            size: '65%',
            background: 'transparent',
            colors: ['#ff9999', '#21BA45', '#9C27B0', '#E91E63', '#F2C037'],
            labels: {
                show: false,
                name: {
                show: true,
                fontSize: '22px',
                fontFamily: 'Helvetica, Arial, sans-serif',
                fontWeight: 600,
                color: undefined,
                offsetY: -10,
                formatter: function (val) {
                    return val
                }
            },
            value: {
                show: true,
                fontSize: '16px',
                fontFamily: 'Helvetica, Arial, sans-serif',
                fontWeight: 400,
                color: undefined,
                offsetY: 16,
                formatter: function (val) {
                    return val
                }
            },
            total: {
                show: false,
                showAlways: false,
                label: 'Total',
                fontSize: '22px',
                fontFamily: 'Helvetica, Arial, sans-serif',
                fontWeight: 600,
                color: '#373d3f',
                formatter: function (w) {
                    return w.globals.seriesTotals.reduce((a, b) => {
                    return a + b
                    }, 0)
                }   
            }
        },
        fill:{
            colors: ['#ff9999', '#21BA45', '#9C27B0', '#E91E63', '#F2C037'],
        }
        },     
    }
    },
    series: [44, 55, 41, 17, 15],
    };
  }
};
</script>

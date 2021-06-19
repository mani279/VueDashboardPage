<template>
  <q-page>
    <div class="q-pa-md">
    <div class="row">
      <div class="col-12">
        <AreaChart/>
      </div>
    </div>
    <div class="row">
      <div class="col-12"><StockCards/></div>
    </div>

    <div class="row">
      <div class="col-xl-8 col-lg-8 col-md-8 col-sm-12 col-xs-12"><Table/></div>
      <div class="col-xl-4 col-lg-4 col-md-4 col-sm-12 col-xs-12"><PieChart/></div>
    </div>

  </div>
  </q-page>
</template>

<script>
import AreaChart from '../components/AreaChart.vue';
import StockCards from '../components/StockCards.vue';
import Table from '../components/Table.vue';
import PieChart from '../components/PieChart.vue'

export default {
  name: 'PageIndex',
  components: {
    AreaChart,
    StockCards,
    Table,
    PieChart
  },
  data: function() {
    return {
      
    }
  },
}
</script>

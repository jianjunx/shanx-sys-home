<template>
  <div class="home">
    <line-chart class="home-item"></line-chart>
    <histogram-chart class="home-item"></histogram-chart>
    <funnel-chart class="home-item"></funnel-chart>
    <map-chart class="home-item"></map-chart>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import LineChart from "./components/LineChart.vue";
import HistogramChart from "./components/HistogramChart.vue";
import FunnelChart from "./components/FunnelChart.vue";
import MapChart from "./components/MapChart.vue";

@Component({
  components: {
    LineChart,
    HistogramChart,
    FunnelChart,
    MapChart,
  },
})
export default class App extends Vue {}
</script>

<style lang="scss">
.home {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: center;
  &-item {
    width: 46%;
    margin-top: 2%;
  }
}
</style>

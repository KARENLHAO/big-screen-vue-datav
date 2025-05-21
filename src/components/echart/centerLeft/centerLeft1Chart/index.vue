<template>
  <div>
    <Chart :cdata="cdata" />
  </div>
</template>

<script>
import Chart from './chart.vue';
export default {
  data () {
    return {
      cdata: {
        xData: ["冲压", "焊接", "涂装", "质检", "总装", "包装出货"],
        seriesData: [
          { value: 10, name: "冲压" },
          { value: 5, name: "焊接" },
          { value: 15, name: "涂装" },
          { value: 25, name: "质检" },
          { value: 20, name: "总装" },
          { value: 35, name: "包装出货" }
        ]
      }
    }
  },
  components: {
    Chart,
  },
  mounted () {
  },
  methods: {
  }
}
</script>

<style lang="scss" scoped>
</style>
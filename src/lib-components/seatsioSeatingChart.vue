<script>
import SeatsioEmbeddable from './seatsioEmbeddable.vue'

export default {
  mixins: [SeatsioEmbeddable],
  name: 'SeatsioSeatingChart',
  methods: {
    createChart: function (seatsio, config) {
      return new seatsio.SeatingChart(config)
    }
  }
}
</script>

<template>
  <div :id="id"></div>
</template>
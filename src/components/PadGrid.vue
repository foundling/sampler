<template>
  <div class="pad-grid">
    <div class="pad-row" v-for="row in rows">
      <pad v-for="pad in rowLength" />
    </div>
  </div>
</template>

<script>

import Pad from '@/components/Pad'

export default {
  name: 'PadGrid',
  data () {
    return {
      rowLength: 4,
      rows: 4
    }
  },
  components: {
    Pad
  },
  methods: {
  }
}
</script>

<style scoped lang="scss">
  .pad {
    display: inline-block;
  }
  .pad-row {
    display: block;
  }
</style>

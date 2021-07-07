<template>
  <div class="current-series">
      <img :src="prod.thumb" :alt="prod.series">
  </div>
</template>

<script>
export default {
    name: 'Series',
    props: ["prod"]
}
</script>

<style>




</style>
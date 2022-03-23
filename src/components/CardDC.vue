<template>
    <div>
      <img :src="cardThumb" :alt="cardSeries">
      <p>{{ cardSeries }}</p>
    </div>
</template>

<script>
export default {
  name: 'CardDC',
  props: {
    cardThumb: String,
    cardSeries: String
  }
}
</script>

<style>

</style>

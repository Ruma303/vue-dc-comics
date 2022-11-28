<template>
  <div class="card">
    <img
      :src="thumb"
      :alt="series"
    >
    <h3>{{ series }}</h3>
  </div>
</template>

<script>
export default {
  name: "CardPage",
  props: {
    thumb: String,
    series: String,
  },
};
</script>

<style lang="scss" scoped>
.card {
  text-align: left;
  flex: 0 0 15%;
}
</style>

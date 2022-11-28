<template>
  <div class="card">
    <img :src="thumb" alt="" />
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
  flex: 0 0 calc((100% / 6) - (100% - 5rem));
  height: 300px;
  width: 200px;
}
</style>

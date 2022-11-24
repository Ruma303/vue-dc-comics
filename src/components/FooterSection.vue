<template>
  <footer>
    <div class="top-footer"></div>
    <div class="middle-footer"></div>
    <div class="bottom-footer"></div>
    <div class="rest-footer"></div>
  </footer>
</template>

<script>
export default {
  name: 'FooterSection',
};
</script>

<style lang="scss" scoped>
  .top-footer{
    background-color: rgb(15, 130, 247);
    height: 189px;
  }
  .middle-footer{
    background-image: url('@/img/footer-bg.jpg');
    height: 490px;
    background-repeat: none;
  }
  .bottom-footer{
    background-color: rgb(47, 47, 47);
    height: 157px;
  }
  .rest-footer{ //FIXME: non compare
    background-color: rgb(32, 32, 32);
    height: 50vh;
  }
</style>

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
    background-color: rgb(15, 130, 247); //FIXME: qui chiamata alla variabile ma non funziona
    height: 189px;//TODO: rendi dinamico
  }
  .middle-footer{
    background-image: url('@/img/footer-bg.jpg');
    height: 480px; //TODO: rendi dinamico
    background-repeat: none;
  }
  .bottom-footer{
    background-color: rgb(47, 47, 47);
    height: 157px;//TODO: rendi dinamico
  }
  .rest-footer{
    background-color: rgb(32, 32, 32);
    height: 50vh;//TODO: rendi dinamico
  }
</style>

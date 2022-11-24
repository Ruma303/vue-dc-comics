<template>
  <div>
    <HeaderSection />
    <MainSection />
    <FooterSection />
  </div>
</template>

<script>
import HeaderSection from '@/components/HeaderSection.vue';
import MainSection from '@/components/MainSection.vue';
import FooterSection from '@/components/FooterSection.vue';

export default {
  components: {
    HeaderSection,
    MainSection,
    FooterSection,
  },
};
</script>

<style lang="scss">
*{
  margin:0; padding: 0; box-sizing: border-box; font-family: 'Roboto', sans-serif;
}
</style>

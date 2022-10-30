<template>
  <div class=" overflow-hidden">
    <subhero />
    <hero/>
    <galleries/>
    <reviewers/>
    <Footer/>
    <!-- <div class=" min-h-[3000px]">ss</div> -->
  </div>
</template>

<script setup>
  import subhero from '@/components/subhero/index.vue';
  import hero from '@/components/hero/index.vue';
  import galleries from '@/components/galleries/index.vue';
  import reviewers from '@/components/reviewers/index.vue';
  import Footer from '@/components/Footer/index.vue';
</script>

<style lang='less' scoped>

</style>
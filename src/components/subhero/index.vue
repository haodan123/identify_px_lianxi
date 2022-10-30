<template>
  <section class="bg-subhero min-h-[715px] bg-no-repeat bg-center relative">
    <div class=" container mx-auto text-white ">
      <!-- header -->
      <Header />
      <!-- 中间的文字和按钮 -->
      <div class="flex flex-col justify-center items-center  gap-10">
        <div class=" mt-[220px] text-5xl font-bold text-center">
          <p class="">Get your creative work reviewed by</p>
          <p class="mt-5">Industry Professionals</p>
        </div>
        <div class="text-center text-2xl px-12 py-3 rounded-full  border-2">
          Get Started
        </div>
      </div>
      <!-- 下面的圆圈勾 -->
      <div
        class=" text-3xl absolute bottom-[-20px] left-[50%] -mt-2 bg-[#FA005E] flex justify-center items-center w-10 h-10 rounded-full">
        &xvee;
      </div>
    </div>
  </section>
</template>

<script setup>
  import Header from '@/components/header/index.vue'
</script>

<style lang='less' scoped>

</style>
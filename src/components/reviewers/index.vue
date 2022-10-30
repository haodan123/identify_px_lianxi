<template>
  <section class="py-[75px] bg-white">

    <div class="container mx-auto">
      <!-- 上面的文字 -->
      <div class="text-black mx-auto text-center mb-16 w-[1000px]">
        <p class="text-5xl font-bold mb-4">Get feedback from industry leaders</p>
        <p class="text-2xl text-gray-500">
          Our platforms brings together some of the best creative people on the planet,
          maybe even the entire universe!
          Take a look at who can give you feedback in the next couple of minutes.
        </p>
      </div>
      <!-- 中间的卡片 -->
      <div class=" flex gap-4">
        <!-- 左边的两个大卡片 -->
        <div class="flex gap-4" v-for="(item,index) in 2" :key="index">
          <div class="w-[390px]  shadow-md rounded-xl">
            <div class=" w-full h-[328px] ">
              <img src="@/assets/images/reviewers/Layer11.png" class="w-full h-full" alt="">
            </div>

            <div class=" p-4">
              <p class="text-2xl">Jessica H. Hanshaw</p>
              <!-- 评分星星 -->
              <div class="flex gap-2 mt-3 items-center">
                <div class="flex gap-1">
                  <img class=" w-[18px] h-[18px]" src="@/assets/images/reviewers/Capa1.png" v-for="(item, index) in 5"
                    :key="index" alt="">
                </div>
                <span class="text-black font-bold text-lg">128</span>
                <span>reviews given</span>
              </div>

              <div class="mt-2 text-gray-600 text-base">
                Nullam ornare lobortis diam vitae elementum. Vestibulu ante ipsum primis in faucibus orci luctus et
                ultrices posu cubilia curae dictum suscipit.
              </div>
              <p class="mt-2 text-[#fa005e] font-bold">WORK WITH DONNA</p>
            </div>
          </div>
        </div>
        <!-- 右边的两个小卡片 -->
        <div class=" flex flex-col gap-4">
          <div class="w-[390px]  shadow-md rounded-xl" v-for="(item, index) in 2" :key="index">
            <div class=" w-full h-[168px]">
              <img src="@/assets/images/reviewers/Layer13.png" alt="">
            </div>
            <div class=" p-4">
              <p class="text-2xl">Jessica H. Hanshaw</p>
              <!-- 评分星星 -->
              <div class="flex gap-2  items-center">
                <div class="flex gap-1">
                  <img class=" w-[18px] h-[18px]" src="@/assets/images/reviewers/Capa1.png" v-for="(item, index) in 5"
                    :key="index" alt="">
                </div>
                <span class="text-black font-bold text-lg">128</span>
                <span>reviews given</span>
              </div>
              <p class="mt-1 text-[#fa005e] font-bold">WORK WITH DONNA</p>
            </div>
          </div>
        </div>
      </div>
      <!-- 下面的文字 -->

      <div class="text-center mt-20 text-black flex justify-center items-center flex-col">
        <p class="text-5xl mb-6 font-bold">
          Are you ready to start your journey?
        </p>
        <div class=" text-white text-2xl px-9 py-3 rounded-full cursor-pointer bg-[#fa005e]">
          Get Started
        </div>
      </div>

    </div>

  </section>
</template>

<script setup>

</script>

<style lang='less' scoped>

</style>
<template>
   <section class="bg-[#fa005e]">
    <div class="py-20 container mx-auto">
      <!-- 文字 -->
      <div class="text-white w-full text-center mb-16">
        <p class="text-5xl font-bold mb-4">Explore our galleries</p>
        <p class="text-2xl">All these entries are taken from Dribbble.com. The authors and entry names are real so feel</p>
      </div>
      <!-- 中间的卡片 -->
      <div class="flex flex-wrap gap-5 mb-20">
        <div class=" overflow-hidden rounded-lg w-[280px]" v-for="(item,index) in galleries" :key="index">
          <div class=" w-full h-[230px]">
            <img :src="item.img" alt="">
          </div>
          <div class=" p-4 bg-white ">
            <p class=" text-2xl">{{item.title}}</p>
            <p class="text-xl text-gray-500">{{item.content}}</p>
          </div>
        </div>
      </div>
      <!-- 下面的文字 -->
      <div class="text-center text-white flex justify-center items-center flex-col">
        <p class="text-5xl mb-6">
          Are you ready to start your journey?
        </p>
        <div class="border-2 text-2xl px-9 py-3 rounded-full cursor-pointer">
          Get Started
        </div>
      </div>
    </div>

   </section>
</template>

<script setup >
import Layer3 from '@/assets/images/galleries/Layer 3.png'
import Layer4 from '@/assets/images/galleries/Layer 4.png'
import Layer5 from '@/assets/images/galleries/Layer 5.png'
import Layer6 from '@/assets/images/galleries/Layer 6.png'
import Layer7 from '@/assets/images/galleries/Layer 7.png'
import Layer8 from '@/assets/images/galleries/Layer 8.png'
import Layer9 from '@/assets/images/galleries/Layer 9.png'
import Layer0 from '@/assets/images/galleries/Layer 10.png'
import { ref } from 'vue'
const galleries = ref([
  {
    img:Layer3,
    title:'Monster Project',
    content:'by Elias Stein'
  },
  {
    img:Layer4,
    title:'Monster Project',
    content:'by Elias Stein'
  },
  {
    img:Layer5,
    title:'Monster Project',
    content:'by Elias Stein'
  },
  {
    img:Layer6,
    title:'Monster Project',
    content:'by Elias Stein'
  },
  {
    img:Layer7,
    title:'Monster Project',
    content:'by Elias Stein'
  },
  {
    img:Layer8,
    title:'Monster Project',
    content:'by Elias Stein'
  },
  {
    img:Layer9,
    title:'Monster Project',
    content:'by Elias Stein'
  },
  {
    img:Layer0,
    title:'Monster Project',
    content:'by Elias Stein'
  }
])

</script>

<style lang='less' scoped>

</style>
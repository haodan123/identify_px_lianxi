<template>
  <section class="bg-white">
    <div class="container mx-auto px-12 pt-20 pb-24">
      <!-- 文字 -->
      <div class="text-center mb-20">
        <p class=" text-4xl font-bold" style="font-family:'Times New Roman', Times, serif">How does Critiq work?</p>
        <p class=" mt-5 text-gray-600 max-w-[997px]">The entire process is incredibly easy: you sign up, you select some
          awesome people
          from that particular field your work belongs to ... and that’s it! Reviews are going to start pouring in.</p>
      </div>
      <!-- 三个图标 -->
      <div class="  flex justify-between">
        <div class=" text-center items-center max-w-80 flex flex-col " v-for="(item, index) in critiqArr"
          :key="index">
          <!-- 图标 -->
          <div
            class=" shadow-md rounded-full w-[135px] h-[135px] border-4 border-[#ff4b1b]  flex justify-center items-center border-solid">
            <img class=" " :src="item.img" alt="">
          </div>
          <!-- 文字 -->
          <div class="mt-7 text-black text-xl">
            {{item.title}}
          </div>
          <div class=" mt-5 text-gray-500 text-sm">
            {{item.content}}
          </div>
          <div class=" font-bold text-lg mt-6 text-[#fa005e]">
            {{item.sub}}
          </div>


        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import Shape1 from '@/assets/images/subhero/Shape 1.png'
import Shape2 from '@/assets/images/subhero/Shape 2.png'
import Shape3 from '@/assets/images/subhero/Shape 3.png'
import { ref } from 'vue';
const critiqArr = ref([{
  img:Shape1,
  title:'Create an account on Critiq',
  content:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum feugiat pellentesque dui molestie lobortis. Vivamus vehicula ante at sapien facilisis.",
  sub:'REGISTER'
},{
  img:Shape2,
  title:'Select professionals that will review your work',
  content:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum feugiat pellentesque dui molestie lobortis. Vivamus vehicula ante at sapien facilisis.",
  sub:'BROWSE PROFESSIONALS'
},{
  img:Shape3,
  title:'Get your feedback and apply it',
  content:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum feugiat pellentesque dui molestie lobortis. Vivamus vehicula ante at sapien facilisis.",
  sub:'CHECK YOUR DATA'
}])

</script>

<style lang='less' scoped>

</style>
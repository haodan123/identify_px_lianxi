<template>
  <header class="fixed top-9 container flex justify-between items-center p-2 bg-black/50 rounded-full">
    <div class=" cursor-pointer"><img src="@/assets/images/header/CRITIQ.png" alt=""></div>
    <div class="flex gap-5 items-center">
      <div class="flex gap-5 cursor-pointer">
        <div @click="active = item.id" :class="{' text-[#909090]':item.id===active}" v-for="(item,index) in navbar" :key="item.id">
        {{item.name}}</div>
      </div>
      <div class="bg-[#fa005e] py-3 px-7 rounded-full cursor-pointer">
        REGISTER
      </div>
    </div>
  </header>
</template>

<script setup>
  import {
    ref
  } from 'vue';
  
  const active = ref(1)

  const navbar = ref([{
    name: 'HOME',
    id: 1
  }, {
    name: ' HOW IT WORKS',
    id: 2
  }, {
    name: 'REVIEWERS',
    id: 3
  }, {
    name: 'WORKBOARD',
    id: 4
  }, {
    name: 'LOGIN',
    id: 5
  }])
</script>

<style lang='less' scoped>

</style>
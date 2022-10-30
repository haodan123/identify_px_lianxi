<template>
  <footer class="">
    <!-- 上面的盒子 -->
    <div class="bg-[#1a1c28] py-20">
      <div class="container mx-auto flex gap-12">
        <!-- 左边的盒子 -->
        <div class=" w-[370px] flex flex-col gap-11">

          <div class=" w-full pb-4 border-b-2 relative  border-gray-600
          ">
            <p class="text-white text-xl">
              <span class=" font-bold mr-2">ABOUT</span>
              <span>US</span>
            </p>
            <div class="absolute left-0 -bottom-0 w-[30%] border-b-2 z-10  border-blue-600 "></div>
          </div>

          <div class="flex gap-5 flex-col">
            <div class="w-[82px] h-[26px]"> <img class=" w-full h-full" src="@/assets/images/footer/CRITIQ.png" alt="">
            </div>
            <p class="text-gray-400">
              Nullam ornare lobortis diam vitae elementum. Vestibulum ante
              ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae;
              Vivamus gravida consectetur vehicula. Aenean imperdiet rutrum
              arcu, quis lacinia quam tristique sit amet. Pellentesque a lorem
              imperdiet, ornare dui.
            </p>
          </div>

          <div class="flex gap-3">
            <img v-for="(item,index) in 5" src="@/assets/images/footer/Forma1.png" alt="">
          </div>
        </div>
        <!-- 中间的盒子 -->
        <div class=" w-[370px] flex flex-col gap-11">

          <div class=" w-full pb-4 border-b-2 relative  border-gray-600
          ">
            <p class="text-white text-xl">
              <span class=" font-bold mr-2">LATEST</span>
              <span>REVIEWERS</span>
            </p>
            <div class="absolute left-0 -bottom-0 w-[30%] border-b-2 z-10  border-blue-600 "></div>
          </div>

          <div>
            <div class="flex flex-wrap gap-3">
              <div class="w-[115px] h-[115px]" v-for="(item, index) in 6" :key="index">
                <img src="@/assets/images/footer/Layer15.png" alt="">
              </div>
            </div>
          </div>

        </div>
        <!-- 右边的盒子 -->

        <div class=" w-[370px] flex flex-col gap-11">

          <div class=" w-full pb-4 border-b-2 relative  border-gray-600">
            <p class="text-white text-xl">
              <span class=" font-bold mr-2">RECENT</span>
              <span>TWEETS</span>
            </p>
            <div class="absolute left-0 -bottom-0 w-[30%] border-b-2 z-10  border-blue-600 "></div>
          </div>

          <div class="flex flex-col gap-7">

            <div class="flex gap-3" v-for="(item,index) in 3">
              <div class="w-7 h-7">
                <img class="w-full h-full" src="@/assets/images/footer/Forma1.png" alt="">
              </div>

              <div class="text-sm text-gray-400 w-[80%]">
                <p>
                  Nullam ornare lobortis diam vitae elementum vestibulu ante ipsum primis in faucibus orci luctus et
                </p>
                <p class="mt-2">
                  50 minutes ago
                </p>
              </div>

            </div>

          </div>

        </div>


      </div>
    </div>
    <!-- 下面的盒子 -->
    <div class="bg-[#141622]">
      <div class="container mx-auto flex justify-between text-white py-6">
        <div>
          <p>Copyright @ <span class="text-[#fa005e]"> thislooksgreat.net.</span> All rights reserved.</p>
        </div>
        <div class="flex gap-5">
          <div v-for="(item, index) in footerbar" :key="index">
            {{item.name}}</div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
  import {
    ref
  } from 'vue';

  const footerbar = ref(
    [{
      name: 'HOME'
    }, {
      name: ' HOW IT WORKS'
    }, {
      name: 'REVIEWERS'
    }, {
      name: 'WORKBOARD'
    }, {
      name: 'LOGIN'
    }]
  )
</script>

<style lang='less' scoped>

</style>
<template>
  <div
    class="w-[calc(33%-58px)] bg-gray-800 h-96 absolute bottom-[1152px] left-0 flex justify-center items-center z-50"
  >
    <div
      class="w-8 h-full bg-blue-600 flex flex-col justify-start items-center"
    >
      <div class="w-full h-8 rounded-full bg-black"></div>
      <div class="w-full h-8 rounded-full bg-black"></div>
      <div class="w-full h-8 rounded-full bg-black"></div>
      <div class="w-full h-8 rounded-full bg-black"></div>
      <div class="w-full h-8 rounded-full bg-black"></div>
      <div class="w-full h-8 rounded-full bg-black"></div>
      <div class="w-full h-8 rounded-full bg-black"></div>
      <div class="w-full h-8 rounded-full bg-black"></div>
      <div class="w-full h-8 rounded-full bg-black"></div>
      <div class="w-full h-8 rounded-full bg-black"></div>
      <div class="w-full h-8 rounded-full bg-black"></div>
      <div class="w-full h-8 rounded-full bg-black"></div>
    </div>
    <TextAnimation
      text="Ohh no Nicholas Latifi"
      size="20"
      color="blue"
      class="absolute right-6 top-6"
    />
    <TextAnimation
      text="No Mickey no <br> That was so not right"
      size="20"
      color="cyan"
      class="absolute right-6 bottom-10"
    />
    <p class="text-xl text-white absolute left-2 top-2">Abu Dhabi 2021</p>
    <Latifi class="absolute top-1/2 -translate-y-1/2 right-44 -rotate-45" />
  </div>
</template>

<script setup>
import TextAnimation from "./TextAnimation.vue";
import Latifi from "./cars/Latifi.vue";
</script>

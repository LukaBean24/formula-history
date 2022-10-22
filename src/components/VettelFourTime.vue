<template>
  <div
    class="w-[calc(33%-59px)] h-96 bg-gray-500 absolute bottom-[768px] left-0 flex justify-center items-center"
  >
    <VettelRedbull
      class="absolute left-1/2 -translate-x-1/2 top-1/2 -translate-y-1/2"
    />
    <TextAnimation
      class="absolute top-16"
      :text="`Sebastian Vettel is 4 time world champion`"
      color="white"
      size="20"
    />
    <p class="text-xl text-white absolute right-2 top-2">India 2013</p>
  </div>
</template>

<script setup>
import TextAnimation from "@/components/TextAnimation.vue";
import VettelRedbull from "./cars/VettelRedbull.vue";
</script>

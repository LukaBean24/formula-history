<template>
  <div
    class="w-[calc(33%-58px)] h-96 bg-gradient-to-b from-red-500 to-yellow-300 absolute bottom-96 left-0 flex justify-center items-center"
  >
    <Leclerc class="absolute right-6 bottom-4" />
    <div class="w-10 h-full bg-gray-400 relative">
      <div
        class="w-10 h-10 bg-black grid grid-cols-3 grid-rows-3 gap-2 absolute left-full top-1/2 -translate-y-1/2"
      >
        <div class="col-span-1 row-span-1 bg-white"></div>
        <div class="col-span-1 row-span-1 bg-white"></div>
        <div class="col-span-1 row-span-1 bg-white"></div>
        <div class="col-span-1 row-span-1 bg-white"></div>
        <div class="col-span-1 row-span-1 bg-white"></div>
        <div class="col-span-1 row-span-1 bg-white"></div>
        <div class="col-span-1 row-span-1 bg-white"></div>
        <div class="col-span-1 row-span-1 bg-white"></div>
        <div class="col-span-1 row-span-1 bg-white"></div>
      </div>
    </div>
    <TextAnimation
      class="absolute top-10"
      :text="`Mercedes threw everything at him today <br> Charles Leclerc coped brilianlly <br> He won in spa HE WINS IN MONZA`"
      color="white"
      size="20"
    />
    <p class="text-xl text-white">Monza 2019</p>
  </div>
</template>

<script setup>
import TextAnimation from "@/components/TextAnimation.vue";
import Leclerc from "./cars/Leclerc.vue";
</script>

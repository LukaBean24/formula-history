<template>
  <div
    class="w-[calc(34%-13px)] h-96 absolute bottom-[1152px] left-[635px] flex justify-center items-center z-50"
  >
    <p class="text-xl text-white absolute left-2 top-32">Spa 2018</p>
    <VettelFerrari class="absolute left-8 -bottom-16" />
    <LewisSilver class="absolute left-32 bottom-0" />
    <TextAnimation
      text="But Here Comes <br> SEBASTIAN VETTEL"
      color="red"
      size="32"
    />
  </div>
</template>

<script setup>
import VettelFerrari from "./cars/VettelFerrari.vue";
import LewisSilver from "./cars/LewisSilver.vue";
import TextAnimation from "./TextAnimation.vue";
</script>

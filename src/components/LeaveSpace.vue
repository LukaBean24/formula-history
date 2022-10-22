<template>
  <div
    class="w-[calc(34%-13px)] h-96 absolute bottom-96 left-[635px] flex justify-center items-center z-50"
  >
    <p class="text-xl text-white absolute left-2 top-32">Bahrein 2012</p>
    <AlonsoFerrari />
    <Rosberg class="absolute right-6 bottom-32" />
    <TextAnimation
      text="Okay he pushed me of the track <br> I think you have to leave the space <br> ALL THE TIME YOU HAVE TO LEAVE A SPACE"
      color="red"
      size="20"
    />
  </div>
</template>

<script setup>
import TextAnimation from "./TextAnimation.vue";
import AlonsoFerrari from "./cars/AlonsoFerrari.vue";
import Rosberg from "./cars/Rosberg.vue";
</script>

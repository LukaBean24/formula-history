<template>
  <div
    class="w-[calc(34%-13px)] h-96 absolute bottom-[768px] left-[635px] flex justify-center items-center z-50"
  >
    <p class="text-xl text-white absolute left-2 top-32">Spain 2016</p>
    <LewisBarcelona />
    <Rosberg class="absolute right-6 bottom-32" />
    <TextAnimation
      text="Hamilton is onto the grass <br> And Hamilton had a massive crash <br> And he crashed into his teammate"
      color="cyan"
      size="20"
    />
  </div>
</template>

<script setup>
import TextAnimation from "./TextAnimation.vue";
import AlonsoFerrari from "./cars/AlonsoFerrari.vue";
import Rosberg from "./cars/Rosberg.vue";
import LewisBarcelona from "./cars/LewisBarcelona.vue";
</script>

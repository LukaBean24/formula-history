<template>
  <div
    class="w-[calc(33%-59px)] h-96 bg-gray-500 absolute bottom-0 left-0 flex justify-center items-center"
  >
    <Senna />
    <Prost />
    <TextAnimation
      :text="`Senna and Prost crashed <br> That's amazing`"
      color="red"
      size="30"
    />
    <p class="text-xl text-white absolute right-2 top-2">Japan 1990</p>
  </div>
</template>

<script setup>
import Senna from "@/components/cars/Senna.vue";
import Prost from "@/components/cars/Prost.vue";
import TextAnimation from "@/components/TextAnimation.vue";
</script>

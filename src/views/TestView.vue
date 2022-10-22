<template>
  <div
    class="w-full h-screen bg-black flex justify-center items-center relative"
  >
    <TextAnimation
      :color="`red`"
      size="16"
      :text="`Senna and Prost Crashed <br> That's amazing`"
    />
  </div>
</template>
<script setup>
import TextAnimation from "@/components/TextAnimation.vue";
</script>

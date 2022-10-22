<template>
  <p
    id="text"
    :style="`color: ${color}; font-size: ${size}px`"
    class="text-center"
    v-html="text"
  ></p>
</template>

<script setup>
const props = defineProps(["text", "color", "size"]);
</script>

<style scoped>
#text {
  animation: text-animation 2s infinite ease-in-out;
}

@keyframes text-animation {
  0% {
    transform: translateY(-20px);
    opacity: 0;
  }
  50% {
    transform: translateY(0);
    opacity: 100%;
  }
  100% {
    transform: translateY(-20px);
    opacity: 0;
  }
}
</style>

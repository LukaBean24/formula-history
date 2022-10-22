<template>
  <div
    class="w-20 h-32 absolute rotate-180"
    :style="`top: ${positionFromTop}px; left: ${positionFromLeft}px; transform: rotate(${rotate}deg);`"
  >
    <div
      class="w-full h-full bg-[#991f00] rounded-t-3xl rounded-b-3xl flex justify-center items-center relative z-20"
    >
      <div class="w-4 h-full bg-black"></div>
      <div
        class="w-14 h-16 bg-black absolute rounded-3xl bottom-3 flex justify-center items-center"
      >
        <div class="w-8 h-8 bg-purple-600 rounded-full"></div>
      </div>
    </div>
    <div class="w-8 h-8 bg-black rounded-full absolute top-4 -right-2"></div>
    <div class="w-8 h-8 bg-black rounded-full absolute top-4 -left-2"></div>
    <div class="w-8 h-8 bg-black rounded-full absolute bottom-4 -right-2"></div>
    <div class="w-8 h-8 bg-black rounded-full absolute bottom-4 -left-2"></div>
  </div>
</template>

<script setup>
import { ref } from "@vue/reactivity";
import { onMounted, watch } from "@vue/runtime-core";

const positionFromTop = ref(7872);
const positionFromLeft = ref(8);
const rotate = ref(0);

window.addEventListener("keydown", (event) => {
  if (event.key === "ArrowUp") {
    if (rotate.value === -90 || rotate.value === 270) {
      event.preventDefault();
      positionFromLeft.value -= 40;
    } else if (rotate.value === 90 || rotate.value === -270) {
      event.preventDefault();
      positionFromLeft.value += 40;
    } else if (rotate.value === -180 || rotate.value === 180) {
      event.preventDefault();
      positionFromTop.value += 40;
    } else if (
      rotate.value === 0 ||
      rotate.value === -360 ||
      rotate.value === 360
    ) {
      positionFromTop.value -= 40;
    } else if (rotate.value < 0 && rotate.value > -90) {
      positionFromTop.value -= 40;
      positionFromLeft.value -= 40;
    } else if (rotate.value > 0 && rotate.value < 90) {
      positionFromTop.value -= 40;
      positionFromLeft.value += 40;
    } else if (rotate.value > 90 && rotate.value < 180) {
      event.preventDefault();
      positionFromTop.value += 40;
      positionFromLeft.value += 40;
    } else if (rotate.value > 180 && rotate.value < 270) {
      event.preventDefault();
      positionFromTop.value += 40;
      positionFromLeft.value -= 40;
    } else if (rotate.value > 270 && rotate.value < 360) {
      event.preventDefault();
      positionFromTop.value -= 40;
      positionFromLeft.value -= 40;
    } else if (rotate.value > 270 && rotate.value < 360) {
      event.preventDefault();
      positionFromTop.value -= 40;
      positionFromLeft.value -= 40;
    }
  }
  //   }
  //   if (event.key === "ArrowDown") {
  //   if (rotate.value === -90) {
  //     event.preventDefault();
  //     positionFromLeft.value += 40;
  //   } else if (rotate.value === 90) {
  //     event.preventDefault();
  //     positionFromLeft.value -= 40;
  //   } else if (rotate.value === -180 || rotate.value === 180) {
  //     event.preventDefault();
  //     positionFromTop.value -= 40;
  //   } else if (rotate.value === 0) {
  //     positionFromTop.value += 40;
  //   } else if (rotate.value > 0 && rotate.value < 90) {
  //     positionFromTop.value += 40;
  //   }
  //   }
  if (event.key === "ArrowLeft") {
    rotate.value -= 15;
  }
  if (event.key === "ArrowRight") {
    rotate.value += 15;
  }
});
watch(rotate, () => {
  console.log(rotate.value + " rotate");
});
watch(positionFromTop, () => {
  console.log(positionFromTop.value + " from top");
  console.log(window.scrollY);
});
</script>

<template>
  <div
    ref="container"
    class="w-full h-[8000px] bg-lime-800 flex justify-center items-center relative overflow-hidden"
  >
    <SennaProst />
    <WinsMonza />
    <VettelFourTime />
    <HereComesSeb />
    <AbuDhabiLatifi />
    <LeaveSpace />
    <BarcelonaMerc />
    <div
      class="w-16 h-full bg-white flex flex-col justify-end items-center space-y-6"
    >
      <div
        v-for="kerb in kerbs"
        :key="kerb"
        class="w-full h-[80px] bg-red-500"
      ></div>
    </div>
    <div class="w-1/3 h-full bg-white grid grid-cols-4 gap-4 relative">
      <div class="col-span-1 h-full bg-zinc-700"></div>
      <div class="col-span-1 h-full bg-zinc-700"></div>
      <div class="col-span-1 h-full bg-zinc-700"></div>
      <div class="col-span-1 h-full bg-zinc-700"></div>
      <UserCar />
    </div>
    <div
      class="w-16 h-full bg-white flex flex-col justify-end items-center space-y-6"
    >
      <div
        v-for="kerb in kerbs"
        :key="kerb"
        class="w-full h-[80px] bg-red-500"
      ></div>
    </div>
  </div>
</template>

<script setup>
import UserCar from "@/components/UserCar.vue";
import { onMounted, ref } from "@vue/runtime-core";
import SennaProst from "@/components/SennaProst.vue";
import WinsMonza from "@/components/WinsMonza.vue";
import VettelFourTime from "../components/VettelFourTime.vue";
import HereComesSeb from "../components/HereComesSeb.vue";
import AbuDhabiLatifi from "../components/AbuDhabiLatifi.vue";
import LeaveSpace from "../components/LeaveSpace.vue";
import BarcelonaMerc from "../components/BarcelonaMerc.vue";

const container = ref();
const kerbs = ref([]);

onMounted(() => {
  setTimeout(() => {
    window.scrollTo(0, 8000);
  }, 1000);
  let i = 0;
  while (i < 100) {
    kerbs.value.push(i);
    i++;
  }
});
</script>

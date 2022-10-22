<template>
  <div class="w-16 h-32" id="car">
    <div
      class="h-full w-full bg-gray-400 rounded-3xl flex justify-center items-center z-30"
    >
      <div
        class="w-14 h-10 rounded-full bg-gray-700 absolute top-12 flex justify-center items-center"
      >
        <div
          class="w-full h-5/6 absolute bottom-0 bg-gray-400 rounded-full flex justify-center items-center"
        >
          <div class="w-2 h-full bg-green-300"></div>
        </div>
      </div>
      <div class="w-2 h-full bg-green-300"></div>
      <div
        class="w-10 h-12 rounded-xl bg-gray-900 absolute bottom-4 flex justify-center items-center"
      >
        <div
          class="w-6 h-6 bg-purple-500 rounded-full flex justify-center items-center"
        >
          <div class="w-1/3 h-full bg-black"></div>
        </div>
      </div>
    </div>
    <div class="w-6 h-6 bg-black absolute bottom-3 -left-3 rounded-full"></div>
    <div class="w-6 h-6 bg-black absolute top-3 -left-3 rounded-full"></div>
    <div class="w-6 h-6 bg-black absolute bottom-3 -right-3 rounded-full"></div>
    <div class="w-6 h-6 bg-black absolute top-3 -right-3 rounded-full"></div>
  </div>
</template>

<style scoped>
#car {
  position: absolute;
  right: -20px;
  bottom: -100px;
  animation: lew infinite 4s ease-in-out;
  transform: rotate(0);
}

@keyframes lew {
  0% {
    right: -20px;
    bottom: -100px;
    transform: rotate(0);
  }
  30% {
    right: -20px;
    bottom: -50px;
    transform: rotate(0);
  }
  70% {
    right: -100px;
    bottom: 0px;
    transform: rotate(0);
  }
  100% {
    right: -50px;
    bottom: 100px;
    transform: rotate(-180deg);
  }
}
</style>

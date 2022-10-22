<template>
  <div class="w-16 h-32 absolute" id="car">
    <div
      class="h-full w-full bg-red-500 rounded-3xl flex justify-center items-center z-30"
    >
      <div
        class="w-14 h-10 rounded-full bg-black absolute top-12 flex justify-center items-center"
      >
        <div
          class="w-full h-5/6 absolute bottom-0 bg-red-500 rounded-full flex justify-center items-center"
        >
          <div class="w-2 h-full bg-white"></div>
        </div>
      </div>
      <div class="w-2 h-full bg-white"></div>
      <div
        class="w-10 h-12 rounded-xl bg-gray-900 absolute bottom-4 flex justify-center items-center"
      >
        <div
          class="w-6 h-6 bg-red-500 rounded-full flex justify-center items-center"
        >
          <div class="w-1/3 h-full bg-red-500 rounded-l-full"></div>
          <div class="w-1/3 h-full bg-yellow-500"></div>
          <div class="w-1/3 h-full bg-red-500 rounded-r-full"></div>
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
  animation: seb infinite 2s ease-out;
  right: 20px;
  bottom: -200px;
}

@keyframes seb {
  0% {
    right: 20px;
    bottom: -200px;
  }
  20% {
    bottom: -100px;
    right: 10px;
  }
  80% {
    bottom: 0;
    right: 0;
  }
  100% {
    right: -40px;
    bottom: 20px;
  }
}
</style>

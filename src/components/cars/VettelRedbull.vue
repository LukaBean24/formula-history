<template>
  <div class="w-16 h-32" id="car">
    <div
      class="h-full w-full bg-slate-900 rounded-3xl flex justify-center items-center z-30"
    >
      <div
        class="w-14 h-10 rounded-full bg-black absolute top-12 flex justify-center items-center"
      ></div>
      <div class="w-2 h-full bg-yellow-400"></div>
      <div
        class="w-10 h-12 rounded-xl bg-slate-800 absolute bottom-4 flex justify-center items-center"
      >
        <div
          class="w-6 h-6 bg-red-500 rounded-full flex justify-center items-center"
        >
          <div class="w-1/3 h-full rounded-l-full bg-yellow-500"></div>
          <div class="w-1/3 h-full bg-black"></div>
          <div class="w-1/3 h-full bg-red-500 rounded-r-full"></div>
        </div>
      </div>
    </div>
    <div class="w-6 h-6 bg-black absolute bottom-3 -left-3 rounded-full"></div>
    <div class="w-6 h-6 bg-black absolute top-3 -left-3 rounded-full"></div>
    <div class="w-6 h-6 bg-black absolute bottom-3 -right-3 rounded-full"></div>
    <div class="w-6 h-6 bg-black absolute top-3 -right-3 rounded-full"></div>
    <div
      class="w-16 h-16 bg-gray-200 absolute -bottom-12 rounded-full animate-pulse"
    ></div>
  </div>
</template>

<style scoped>
#car {
  animation: drift 3s infinite ease-in-out;
}

@keyframes drift {
  0% {
    transform: rotate(0deg);
  }
  50% {
    transform: rotate(360deg);
  }
  100% {
    transform: rotate(0deg);
  }
}
</style>

<script setup>
</script>

<template>
  <section class="pt-18 py-20 font-inter" id="hero">
    <!-- <p
      class="border border-cyan-500 px-2 -z-10 rounded-xl mb-5 flex items-center justify-center text-xs lg:text-sm w-fit m-auto animate-scale"
    >
      Available for hire 💡
    </p> -->
    <p class="font-mono pb-3 text-cyan-500">Jambo, I'm</p>
    <h1 class="font-inter pb-4 text-5xl sm:text-6xl text-[#dcd5d1] font-bold">
      Kennedy Otieno.
    </h1>
    <h2 class="font-inter pb-4 font-bold text-zinc-500 text-4xl sm:text-5xl">
      I ensure software is reliable and ready for production.
    </h2>
    <p class="sm:w-1/2 w-full text-lg pb-6">
      I help teams catch issues early by validating user flows, system
      behaviour, and release readiness. My work reduces production
      bugs, improves product stability, and helps teams ship with confidence.
    </p>
  </section>
</template>

<style scoped>
@keyframes scale {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.2);
  }
  100% {
    transform: scale(1);
  }
}

.animate-scale {
  animation: scale 2s infinite;
}
</style>

<script setup>
import resume from "../assets/resume/Kennedy_Resume.pdf";
function downloadResume() {
  const resumeUrl = resume;
  const link = document.createElement("a");
  link.href = resumeUrl;
  link.setAttribute("download", "Kennedy Otieno's resume.pdf");
  link.click();
}
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
      I engineer software solutions that are reliable, and scalable.
    </h2>
    <p class="sm:w-1/2 w-full text-lg pb-6">
      I help companies bridge the gap between design and functionality by
      building interactive user interfaces and robust APIs. My approach
      ensures products are scalable, reliable, efficient, and aligned with
      business goals.
    </p>
    <button
      @click="downloadResume"
      aria-label="This button is responsible for downloading my resume"
      class="px-5 py-3 border border-cyan-500 rounded hover:bg-cyan-500 hover:text-zinc-800 transition-all eas duration-200"
    >
      View my resume 🔎
    </button>
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

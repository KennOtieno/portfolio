<script setup>
import GithubIcon from "./icons/GithubIcon.vue";
import GmailIcon from "./icons/GmailIcon.vue";
import LinkedInIcon from "./icons/LinkedInIcon.vue";
</script>

<template>
  <footer
    class="flex justify-center flex-col rounded-t-md items-center py-2 bg-[#252525] text-sm md:text-base"
  >
    <p class="flex items-center text-center">Find me here 👇</p>
    <div class="grid grid-cols-3 gap-2 pt-1 place-items-center">
      <a
        href="https://github.com/KennOtieno"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="View my Github page"
        ><GithubIcon class="transition-all duration-300 hover:text-cyan-500"
      /></a>
      <a
        href="mailto:kennedyotieno.data@gmail.com"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="Reach out to me on email"
        ><GmailIcon class="transition-all duration-300 hover:text-cyan-500"
      /></a>
      <a
        href="https://www.linkedin.com/in/kennedy-otieno/"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="Link to my linkedIn"
        ><LinkedInIcon class="transition-all duration-300 hover:text-cyan-500"
      /></a>
    </div>
  </footer>
</template>

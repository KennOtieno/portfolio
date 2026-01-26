<script setup>
import BulbIcon from "./icons/BulbIcon.vue";
import LinkIcon from "./icons/LinkIcon.vue";
import GithubIcon from "./icons/GithubIcon.vue";

const tools = [
  {
    id : 6,
    name: "Playwright"
  },

  {
    id: 1,
    name: "Web Testing"
  },

  {
    id: 4,
    name: "API Testing"
  },

  {
    id: 5,
    name: "Appium"
  },

  {
    id: 3,
    name: "Postman"
  },

  {
    id: 2,
    name: "Typescript"
  },
];
</script>

<template>
  <section class="pb-24 font-inter text-base" id="projects">
    <h2 class="font-inter text-cyan-500 text-2xl pb-10">
      Projects
    </h2>

    <div
      class="grid grid-cols-1 md:top-0 mb-28 relative lg:grid-cols-2 gap-4"
      data-aos="fade-up"
      data-aos-anchor-placement="bottom-bottom"
      data-aos-duration="600"
      data-aos-easing="linear"
    >
      <div class="relative group">
        <img
          class="w-full h-5/6 md:mr-auto rounded md:self-center cursor-pointer ease-linear hover:-translate-x-4 hover:translate-y-4 transition-all duration-200"
          src="../assets/orangehrm.png"
          alt="Screenshot of Orangehrm website"
        />
        <div
          class="absolute -z-10 rounded inset-0 border-4 h-5/6 border-cyan-500 transform transition-all duration-300 group-hover:bg-cyan-500"
        ></div>
      </div>

      <div class="py-4 md:p-0 bg-inherit rounded-md">
        <h2 class="font-bold text-xl text-end text-cyan-500">Jadoo</h2>

        <p
          class="bg-inherit py-4 text-up w-full text-end md:w-5/6 md:ml-auto md:p-0 md:pb-4"
        >
          End-to-end UI automation of core OrangeHRM workflows using Playwright (TypeScript).
          Covered authentication, dashboard validation, and PIM employee management
          (add, search, edit). Implemented Page Object Model (POM) for scalable test design,
          used reliable locator strategies, and validated behavior through clear, user focused
          UI assertions.
        </p>
        <div class="grid md:gap-0">
          <ul
            class="font-mono sm:pt-6 md:text-inherit pt-8 flex flex-wrap items-center justify-end gap-4"
          >
            <li class="flex items-center">
              <BulbIcon class="text-cyan-500" /> Vue.js
            </li>
            <li class="flex items-center">
              <BulbIcon class="text-cyan-500" /> Tailwind CSS
            </li>
          </ul>
        </div>

        <div class="flex justify-end pt-10">
          <a
            aria-label="View Github"
            href="https://github.com/KennOtieno/playwright-orangehrm-web-tests"
            target="_blank"
            rel="noopener noreferrer"
            class="hover:text-cyan-500 flex items-end gap-2 text-sm transition-all duration-200"
            ><LinkIcon />View Github</a
          >
        </div>
      </div>
    </div>

    <div
      class="grid grid-cols-1 relative lg:grid-cols-2 gap-4 mb-28"
      data-aos="fade-up"
      data-aos-anchor-placement="bottom-bottom"
      data-aos-duration="700"
      data-aos-easing="linear"
    >
      <div class="py-4 md:p-0 bg-inherit rounded-md order-last lg:order-first">
        <span
          class="text-zinc-900 px-2 text-sm rounded-2xl bg-cyan-100 border-2 border-cyan-100 mb-2"
          >Featured project</span
        >
        <h2 class="font-bold text-xl pb-2 text-cyan-500">
          Password Generator CLI
        </h2>

        <p class="bg-inherit py-4 w-full md:w-5/6 md:p-0 md:pb-4">
          A lightweight command line tool that generates secure passwords
          based on user defined options. Users can specify password length,
          include special characters, and control complexity using command
          line flags.Built with Go for speed, simplicity, and cross
          platform support.
        </p>

        <div class="grid md:gap-0">
          <ul
            class="font-mono sm:pt-6 md:text-inherit pt-8 flex flex-wrap items-center justify-start gap-4"
          >
            <li class="flex items-center">
              <BulbIcon class="text-cyan-500" /> Go
            </li>
          </ul>
        </div>

        <div class="flex justify-start gap-5 pt-10">
          <a
            aria-label="View this project on Github"
            href="https://github.com/KennOtieno/password_generator_cli"
            target="_blank"
            rel="noopener noreferrer"
            class="hover:text-cyan-500 flex items-end gap-2 text-sm transition-all duration-200"
            ><GithubIcon />View on Github</a
          >
        </div>
      </div>
      <div class="relative group order-first lg:order-last">
        <img
          class="w-full h-full md:mr-auto rounded md:self-center cursor-pointer ease-linear hover:-translate-x-4 hover:translate-y-4 transition-all duration-200"
          src="../assets/passwordcli.png.jpg"
          alt="Screenshot of Password Generator CLI "
        />
        <div
          class="absolute -z-10 rounded inset-0 border-4 border-cyan-500 transform transition-all duration-300 group-hover:bg-cyan-500"
          style="height: 100%"
        ></div>
      </div>
    </div>
  </section>
</template>
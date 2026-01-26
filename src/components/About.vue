<script setup>
import BulbIcon from "./icons/BulbIcon.vue";
const tools = [
  {
    id: 6,
    name: "Typescript",
  },
  {
    id: 9,
    name: "JavaScript",
  },
  {
    id: 1,
    name: "Python",
  },

  {
    id: 4,
    name: "Playwright",
  },
  {
    id: 5,
    name: "Test Management",
  },
  {
    id: 3,
    name: "Git",
  },
  {
    id: 2,
    name: "Appium",
  },
  {
    id: 7,
    name: "Cypress",
  },
  {
    id: 8,
    name: "Postman",
  },
];
</script>

<template>
  <section
    class="py-28 font-inter"
    id="about"
    data-aos="flip-left"
    data-aos-easing="linear"
    data-aos-duration="700"
  >
    <h2 class="text-cyan-500 text-2xl pb-10">About me</h2>

    <article
      class="grid sm:grid-cols-2 grid-cols-1 gap-10 justify-items-center place-items-center"
    >
      <img
        class="md:mr-auto rounded"
        src="../assets/codingGuy.gif"
        alt="Animated coding GIF"
      />

      <div>
        <p>
          I’m a Software QA Engineer with hands on experience in manual and automation testing for web & mobile applications. 
          I focus on identifying real product  risks early, improving release quality, and ensuring features behave
          as intended from a user and business perspective.
          Comfortable working with developers, CI pipelines, and fast moving product teams.
          Here are a couple of technologies I have been working with:
        </p>
        <div class="grid grid-cols-2 gap-4 md:gap-0">
          <ul class="font-mono pt-4" v-for="tool in tools" :key="tool.id">
            <li class="flex items-center">
              <BulbIcon class="text-cyan-500" /> {{ tool.name }}
            </li>
          </ul>
        </div>
      </div>
    </article>
  </section>
</template>

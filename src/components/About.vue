<script setup>
import BulbIcon from "./icons/BulbIcon.vue";
const tools = [
  {
    id: 6,
    name: "Django",
  },
  {
    id: 9,
    name: "Laravel",
  },
  {
    id: 1,
    name: "Python",
  },

  {
    id: 4,
    name: "Nuxt.js",
  },
  {
    id: 5,
    name: "Typescript",
  },
  {
    id: 3,
    name: "PHP",
  },
  {
    id: 2,
    name: "Flutter",
  },
  {
    id: 7,
    name: "SQL",
  },
  {
    id: 8,
    name: "Redis",
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
          I’m a Software Engineer who builds scalable, reliable, and user focused applications
          that help businesses run smarter. I specialize in designing effecient backends, creating
          seamless user interfaces, and optimizing systems for perfomance and growth. With hands
          on experience in various technologies, I translate business needs into practical software
          solutions that deliver real impact. Here are a couple of technologies I have been working with:
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

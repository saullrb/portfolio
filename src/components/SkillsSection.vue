<script setup>
import SkillCard from "./SkillCard.vue";

const skills = [
  {
    name: "PHP",
    imgName: "php/php-original.svg",
  },
  {
    name: "Laravel",
    imgName: "laravel/laravel-original.svg",
  },
  {
    name: "Vue",
    imgName: "vuejs/vuejs-original.svg",
  },
  {
    name: "Java",
    imgName: "java/java-original.svg",
  },
  {
    name: "Spring",
    imgName: "spring/spring-original.svg",
  },
  {
    name: "Angular",
    imgName: "angular/angular-original.svg",
  },
  {
    name: "Javascript",
    imgName: "javascript/javascript-original.svg",
  },
  {
    name: "Go",
    imgName: "go/go-original.svg",
  },
  {
    name: "HTML",
    imgName: "html5/html5-original.svg",
  },
  {
    name: "CSS",
    imgName: "css3/css3-original.svg",
  },
  {
    name: "TailwindCSS",
    imgName: "tailwindcss/tailwindcss-original.svg",
  },
  {
    name: "PostgreSQL",
    imgName: "postgresql/postgresql-original.svg",
  },
  {
    name: "Docker",
    imgName: "docker/docker-original.svg",
  },
  {
    name: "Linux",
    imgName: "linux/linux-original.svg",
  },
];
</script>
<template>
  <section id="skills" class="py-20 px-4">
    <div class="max-w-6xl mx-auto space-y-10">
      <h2
        class="font-bold from-primary to-secondary text-center bg-gradient-to-r bg-clip-text text-4xl text-transparent"
      >
        Skills & Technologies
      </h2>
      <div class="grid grid-cols-2 md:grid-cols-3 gap-8 justify-items-center">
        <SkillCard v-for="skill in skills" :key="skill.name" :skill="skill" />
      </div>
    </div>
  </section>
</template>

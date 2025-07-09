<script setup lang="ts">
import ProjectCard from "./ProjectCard.vue";

const projects = [
  {
    title: "ChordPlay",
    description:
      "App to display lyrics with synced chords, for playing or learning songs",
    imageUrl:
      "https://images.unsplash.com/photo-1536594527669-2f555de54e95?q=80&w=1470&auto=format&fit=crop",
    tags: ["PHP", "Laravel", "Vue", "TailwindCSS", "PostgreSQL"],
    repoName: "chordplay",
    url: "https://chordplay.alwaysdata.net",
  },
  {
    title: "LABMedicine Backend",
    description: "API for hospital management system",
    imageUrl:
      "https://images.unsplash.com/photo-1576091160550-2173dba999ef?q=80&w=1470&auto=format&fit=crop",
    tags: ["Java", "Spring", "Oracle"],
    repoName: "LABMedicine-Performance-Backend",
  },
  {
    title: "LABMedicine Frontend",
    description: "Hospital management system",
    imageUrl:
      "https://images.unsplash.com/photo-1681505512385-8b9d567a56c0?q=80&w=1470&auto=format&fit=crop",
    tags: ["Typescript", "Angular", "Bootstrap"],
    repoName: "LABMedicine-Performance-Frontend",
  },
  {
    title: "ytmusiclist",
    description: "CLI program to download YouTube playlists as mp3",
    imageUrl:
      "https://images.unsplash.com/photo-1642659971434-dc73ee111e6f?q=80&w=1470&auto=format&fit=crop",
    tags: ["Go", "FFmpeg", "YT-DLP"],
    repoName: "ytmusiclist",
  },
];
</script>

<template>
  <section id="projects" class="py-20 px-4">
    <div class="max-w-6xl mx-auto space-y-10">
      <h2
        class="font-bold to-secondary from-primary text-center bg-gradient-to-r bg-clip-text text-4xl text-transparent"
      >
        Featured Projects
      </h2>

      <div
        class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-2 gap-8 justify-items-center"
      >
        <ProjectCard
          v-for="project in projects"
          :key="project.title"
          :project="project"
        />
      </div>
    </div>
  </section>
</template>

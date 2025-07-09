<script setup>
import Footer from "./components/Footer.vue";
import HeroSection from "./components/HeroSection.vue";
import Navbar from "./components/Navbar.vue";
import ProjectsSection from "./components/ProjectsSection.vue";
import SkillsSection from "./components/SkillsSection.vue";
</script>

<template>
  <Navbar />

  <main class="space-y-20">
    <HeroSection />
    <ProjectsSection />
    <SkillsSection />
  </main>

  <Footer />
</template>

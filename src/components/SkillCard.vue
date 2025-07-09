<script setup>
defineProps({
  skill: Object,
});

const baseImgUrl = "https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/";
</script>
<template>
  <div
    class="card bg-base-100 w-full group border border-transparent hover:border-base-content/30 transition-all duration-300"
  >
    <div class="card-body items-center text-center">
      <img
        :src="baseImgUrl + skill.imgName"
        :alt="skill.name"
        class="size-12 group-hover:scale-110 transition-transform duration-300"
      />

      <h3
        class="card-title group-hover:brightness-110 transition-all duration-300"
      >
        {{ skill.name }}
      </h3>
    </div>
  </div>
</template>

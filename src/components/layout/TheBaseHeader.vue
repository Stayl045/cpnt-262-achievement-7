<template>
  <header
    class="flex gap-4 bg-blue-300 py-4 justify-items-center shadow-lg shadow-slate-400"
  >
    <TheLogo />
    <TheNavBar />
  </header>
</template>

<script setup>
  import TheNavBar from "@/components/utilities/TheNavBar.vue";
  import TheLogo from "@/components/layout/TheLogo.vue";
</script>

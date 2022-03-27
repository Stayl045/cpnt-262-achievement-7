<template>
  <article
    class="backgroundImage grid text-center content-center rounded-md shadow-lg shadow-slate-400"
  >
    <base-card-title>Howls Moving Castle</base-card-title>
    <BaseCardImage />
    <BaseCardText />
    <BaseCardButton />
  </article>
</template>

<script setup>
  import BaseCardTitle from "@/components/card/card-1/BaseCardTitle.vue";
  import BaseCardImage from "@/components/card/card-1/BaseCardImage.vue";
  import BaseCardText from "@/components/card/card-1/BaseCardText.vue";
  import BaseCardButton from "@/components/utilities/BaseCardButton.vue";
</script>

<style scoped>
  .backgroundImage {
    height: 60vh;
    min-width: 25vw;
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    background-image: url(../../../assets/images/howl.jpg);
  }
</style>

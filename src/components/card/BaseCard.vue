<template>
  <Article
    class="backgroundImage grid text-center content-center m-5 gap-2 rounded-md"
  >
    <base-card-title class="mt-20">Howls Moving Castle</base-card-title>
    <BaseCardImage />
    <BaseCardText />
    <BaseCardButton />
  </Article>
</template>

<script setup>
  import BaseCardTitle from "./BaseCardTitle.vue";
  import BaseCardImage from "./BaseCardImage.vue";
  import BaseCardText from "./BaseCardText.vue";
  import BaseCardButton from "./BaseCardButton.vue";
</script>

<style scoped>
  .backgroundImage {
    height: 50vh;
    width: 50vw;
    background-size: cover;
    background-image: url(../../assets/images/howl-image.jpg);
  }
</style>

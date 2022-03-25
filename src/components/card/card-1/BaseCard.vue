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
  import BaseCardTitle from "@/components/card/card-1/BaseCardTitle.vue";
  import BaseCardImage from "@/components/card/card-1/BaseCardImage.vue";
  import BaseCardText from "@/components/card/card-1/BaseCardText.vue";
  import BaseCardButton from "@/components/card/card-1/BaseCardButton.vue";
</script>

<style scoped>
  .backgroundImage {
    height: 35vh;
    width: 25vw;
    background-size: cover;
    background-image: url(../../../assets//images/howl-image.jpg);
  }
</style>

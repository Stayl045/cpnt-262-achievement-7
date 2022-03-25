<template>
  <article>
    <TheBaseHeader />
    <BaseCard />
  </article>
</template>

<script setup>
  import { computed } from "vue";
  import TheBaseHeader from "./components/layout/TheBaseHeader.vue";
  import BaseCard from "@/components/card/card-1/BaseCard.vue";

  // const cards = [
  //   {
  //     title: "My Neighbor Totoro",
  //     description: "A film about a weird, but lovable creature!",
  //     image: require("@/assets/images/totoro"),
  //   },
  //   {
  //     title: "Ponyo",
  //     description:
  //       "The daughter of a masterful wizard and a sea goddess, Ponyo uses her father's magic to transform herself into a young girl",
  //     image: require("@/assets/images/ponyo"),
  //   },
  // ];
</script>

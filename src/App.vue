<template>
  <article>
    <TheBaseHeader />
    <section class="flex flex-wrap justify-center gap-16 bg-contain mt-16">
      <BaseCard />

      <TheBaseCard v-for="card in cards" :key="card.id">
        <TheCardTitle>{{ card.title }}</TheCardTitle>
        <TheCardDescription>{{ card.description }}</TheCardDescription>
        <TheCardImage :path="card.image.backgroundImage" />
      </TheBaseCard>
    </section>
  </article>
</template>

<script setup>
  import { computed } from "vue";
  import TheBaseHeader from "./components/layout/TheBaseHeader.vue";
  import BaseCard from "./components/card/card-1/BaseCard.vue";
  import TheBaseCard from "./components/card/card-2/TheBaseCard.vue";
  import TheCardTitle from "./components/card/card-2/TheCardTitle.vue";
  import TheCardDescription from "./components/card/card-2/TheCardDescription.vue";
  import TheCardImage from "./components/card/card-2/TheCardImage.vue";

  const cards = [
    {
      title: "My Neighbor Totoro",
      description: "A film about a weird, but lovable creature!",
      image: { backgroundImage: "https://www.ghibli.jp/gallery/totoro022.jpg" },
    },
    {
      title: "Ponyo",
      description:
        "The daughter of a masterful wizard and a sea goddess, Ponyo uses her father's magic to transform herself into a young girl",
      image: { backgroundImage: "https://www.ghibli.jp/gallery/ponyo009.jpg" },
    },
    {
      title: "Spirited Away",
      description: "Daughter goes on a magical adventure to save her parents",
      image: {
        backgroundImage: "https://www.ghibli.jp/gallery/chihiro045.jpg",
      },
    },
  ];
</script>

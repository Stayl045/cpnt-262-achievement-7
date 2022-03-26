<template>
  <article>
    <TheBaseHeader />
    <section
      class="flex flex-wrap justify-center text-center justify-items-center gap-20 bg-cover mt-16 rounded-md mb-10"
    >
      <BaseCard />

      <TheBaseCard v-for="card in cards" :key="card.id" class="rounded-md">
        <TheCardImage :path="card.image.backgroundImage" />
        <TheCardTitle>{{ card.title }}</TheCardTitle>
        <TheCardDescription>{{ card.description }}</TheCardDescription>
        <BaseCardButton />
      </TheBaseCard>
    </section>
    <TheFooter />
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
  import BaseCardButton from "./components/utilities/BaseCardButton.vue";
  import TheFooter from "./components/utilities/TheFooter.vue";

  const cards = [
    {
      title: "My Neighbor Totoro",
      description: "A film about a weird, but lovable creature!",
      image: { backgroundImage: "https://www.ghibli.jp/gallery/totoro022.jpg" },
    },
    {
      title: "Ponyo",
      description:
        "Ponyo uses her father's magic to transform herself into a young girl",
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

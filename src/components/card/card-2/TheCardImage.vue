<template>
  <img
    :src="props.path"
    :alt="props.altText"
    class="rounded-t-lg shadow-lg shadow-slate-300 h-56"
  />
</template>

<script setup>
  import TheCardDescription from "@/components/card/card-2/TheCardDescription.vue";
  import TheCardTitle from "@/components/card/card-2/TheCardTitle.vue";
  const props = defineProps({
    path: {
      type: String,
      required: true,
    },
    altText: {
      type: String,
    },
  });
</script>

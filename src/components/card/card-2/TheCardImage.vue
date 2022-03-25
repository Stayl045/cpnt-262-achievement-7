<template>
  <img :src="props.path" :alt="props.altText" />
</template>

<script setup>
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

<template>
  <iframe
    :src="`https://player.vimeo.com/video/${props.videoId}`"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen
    frameborder="0"
    height="315"
    title="Video player"
    width="460"
  ></iframe>
</template>

<script lang="ts" setup>
const props = defineProps({
  videoId: {
    type: Number,
    required: true
  }
});
</script>

<style scoped></style>

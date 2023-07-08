<template>
  <NuxtLink
    :href="firstLesson.path"
    class="underline font-medium"
  >
    Go to first lesson
  </NuxtLink>
</template>

<script lang="ts" setup>
const firstLesson = await useFirstLesson();
</script>

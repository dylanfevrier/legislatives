<script setup lang="ts">
import {useAsyncData} from "#app";

const { data } = await useAsyncData('statement', () => queryContent('/', '_statement').findOne())
</script>

<template>
  <section>
    <div class="prose md:prose-lg">
      <ContentRendererMarkdown :value="data" />
    </div>
  </section>
</template>

<style scoped>

</style>
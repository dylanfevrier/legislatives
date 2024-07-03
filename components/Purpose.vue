<script setup lang="ts">
import {useAsyncData} from "#app";

const { data } = await useAsyncData('purpose', () => queryContent('/', '_purpose').findOne())
</script>

<template>
  <section>
    <h2 class="mb-5">Mes 12 propositions pour les Francais de l'Etranger</h2>

    <div class="prose md:prose-lg">
      <ContentRendererMarkdown :value="data" />
    </div>
  </section>
</template>

<style scoped>

</style>
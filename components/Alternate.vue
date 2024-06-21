<script setup lang="ts">
import {useAsyncData} from "#app";

const { data } = await useAsyncData('alternate', () => queryContent('/applicants', '_alternate').findOne())
</script>

<template>
  <div>
    <div class="flex">
      <div>
        <div class="flex align-items mb-2">
          <img class="rounded profile" src="~/assets/images/morgane.jpeg" alt="Photo Oussama Laraichi" height="100" />

          <div class="ml-2">
            <span>Suppléante</span>
            <h2>{{ data.name }}</h2>
            <a class="underline" target="_blank" href="https://x.com/morganemrolland">Twitter</a>
          </div>
        </div>

        <ContentRendererMarkdown class="prose md:prose-lg" :value="data" />
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>
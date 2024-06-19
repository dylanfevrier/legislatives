<script setup lang="ts">
import {useAsyncData} from "#app";

const { data } = await useAsyncData('alternate', () => queryContent('/applicants', '_alternate').findOne())
</script>

<template>
  <div>
    <div class="flex">
      <div>
        <div class="flex align-items mb-2">
          <img class="rounded" src="~/assets/images/morgane.jpeg" alt="Photo Oussama Laraichi" width="100px" />

          <div class="ml-2">
            <span>Suppléante</span>
            <h2 class="mb-2">{{ data.name }}</h2>
          </div>
        </div>

        <ContentRendererMarkdown class="prose md:prose-lg" :value="data" />
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>
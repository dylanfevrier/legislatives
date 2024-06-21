<script setup lang="ts">
import {useAsyncData} from "#app";

const { data } = await useAsyncData('applicant', () => queryContent('/applicants', '_applicant').findOne())
</script>

<template>
  <div>
    <div class="flex">
      <div>
        <div class="flex align-items mb-2">
          <img class="rounded profile" src="~/assets/images/oussama.jpeg" alt="Photo Oussama Laraichi" height="100" />

          <div class="ml-2">
            <span>Candidat</span>
            <h2>{{ data.name }}</h2>
            <a class="underline" target="_blank" href="https://x.com/ousslaraichi">Twitter</a>
          </div>
        </div>

        <ContentRendererMarkdown class="prose md:prose-lg" :value="data" />
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>
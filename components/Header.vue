<script setup lang="ts">
import {useAsyncData} from "#app";

const { data } = await useAsyncData('header', () => queryContent('/', '_header').findOne())
</script>

<template>
  <header class="py-3 bg-red">
    <div class="content">
      <div class="w-full text-white text-center">
        <span class="font-semibold">Élections législatives 2024</span> · Votez les  <span class="font-semibold">{{ data.first_round_date }}</span> et  <span class="font-semibold">{{ data.second_round_date }}</span> !
      </div>
    </div>
  </header>
</template>

<style scoped>

</style>
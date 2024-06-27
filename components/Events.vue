<script setup lang="ts">
const events = [
  {
    date: "Jeudi 27 juin",
    link: "https://lu.ma/gs9dowoy",
    title: "Réunion publique à Montréal",
  }
]
</script>

<template>
  <section>
    <div class="mb-5">
      <h1>Prochains événements</h1>
      <div>Les évènements du second tour seront ajoutés bientôt</div>
    </div>

    <div v-for="(event, index) in events" :key="index" class="flex flex-col lg:flex-row lg:justify-between lg:items-center mb-4 gap-y-2">
      <div>
        <span>{{ event.date }}</span>
        <h2>{{ event.title }}</h2>
      </div>

      <a :href="event.link" target="_blank" class="btn btn-outline">Je participe</a>
    </div>


  </section>
</template>
<script setup lang="ts">
</script>
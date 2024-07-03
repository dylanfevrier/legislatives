<script setup lang="ts">
const events = [
  {
    date: "Mercredi 3 juillet",
    link: "https://us06web.zoom.us/j/88079639508?pwd=0l33H4wbnt5I47r7wHkg7Yvf6Qkvh0.1",
    title: "Webinaire Côte Est et France Métropolitaine ",
  },
  {
    date: "Mercredi 3 juillet",
    link: "https://us06web.zoom.us/j/88079639508?pwd=0l33H4wbnt5I47r7wHkg7Yvf6Qkvh0.1",
    title: "Rencontre avec Oussama à Montréal",
  },
  {
    date: "Jeudi 4 juillet",
    link: "https://lu.ma/hwwpezsl ",
    title: "Barbecue républicain et rencontre avec Morgane au Rock Creek Park",
  },
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
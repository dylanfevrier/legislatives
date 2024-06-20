<script setup lang="ts">
const events = [
  {
    date: "Lundi 24 juin",
    link: "https://lu.ma/2f97c6fx",
    title: "Réunion publique à Chicago",
  },
  {
    date: "Mardi 25 juin",
    link: "https://us06web.zoom.us/webinar/register/WN_vECAkhaXQ7m9SOLUnx6eJQ",
    title: "Webinaire (en ligne)",
  },
  {
    date: "Mercredi 26 juin",
    link: "https://lu.ma/ee4pbs12",
    title: "Réunion publique à New York",
  },
  {
    date: "Jeudi 27 juin",
    link: "https://lu.ma/gs9dowoy",
    title: "Réunion publique à Montréal",
  }
]
</script>

<template>
  <section>
    <h1 class="mb-5">Prochains événements</h1>

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
<script setup lang="ts">
const posts = [
  {
    href: "https://frenchmorning.com/oussama-laraichi-nouveau-front-populaire-nous-sommes-le-vote-utile/",
    title: "French Morning",
  },
  {
    href: "https://lepetitjournal.com/expat-politique/actualites/legislatives-2024-oussama-laraichi-nfp-tres-proche-de-ma-circonscription-388514",
    title: "Le Petit Journal",
  },
  {
    href: "https://ici.radio-canada.ca/ohdio/premiere/emissions/phare-ouest/segments/rattrapage/1792377/entrevue-avec-oussama-laraichi-rencontre-candidat-nouveau-front-populaire",
    title: "Radio Canada, Emission Phare Ouest",
  },
  {
    href: "https://www.liberation.fr/international/amerique/le-nouveau-front-populaire-a-lassaut-de-lamerique-du-nord-20240627_Z2HHPJKR2RHY7K4DNX4VJ34TRM/",
    title: "Libération",
  },
  {
    href: "https://www.youtube.com/watch?v=v00eIOTuj7I&ab_channel=%C3%80gauche",
    title: "A Gauche - Youtube",
  },
]
</script>

<template>
  <div class="bg-pink">
    <div class="px-4 w-full lg:w-[1200px] mx-auto py-10 flex flex-col lg:items-center gap-y-4">
      <h2 class="text-white">Oussama Laraichi dans la presse</h2>

      <div class="text-white flex flex-col gap-y-1 lg:justify-center lg:items-center">
        <a
            v-for="(post, index) in posts"
            :key="index"
            class="underline cursor-pointer block"
            :href="post.href"
            target="_blank"
        >
          {{ post.title }}
        </a>
       </div>

      <div class="flex flex-col lg:flex-row gap-x-2 gap-y-2">
        <a href="https://forms.gle/stGrj4PHCEK8X3DWA" target="_blank" class="btn btn-outline">Contact presse</a>
      </div>
    </div>
  </div>
</template>
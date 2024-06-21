<template>
  <div>
    <Header  />

    <Nav class="px-4 w-full lg:w-[1200px] mx-auto mt-2 mb-10 lg:mb-15" />

    <Hero class="px-4 w-full lg:w-[1200px] mx-auto my-10 lg:my-15" />

    <Statement id="statement" class="px-4 w-full lg:w-[1200px] mx-auto my-10 lg:my-15" />

    <Campaign class="my-10 lg:my-15"/>

    <div id="applicant" class="px-4 w-full lg:w-[1200px] mx-auto flex flex-col lg:flex-row gap-x-6 gap-y-4 my-5 lg:my-15">
      <Applicant class="w-full lg:w-1/2" />
      <Alternate class="w-full lg:w-1/2"/>
    </div>

    <Press class="my-10 lg:my-15"/>

    <Events id="events" class="px-4 w-full lg:w-[1200px] mx-auto my-10 lg:my-15" />

    <Footer />
  </div>
</template>
<script setup lang="ts">
import Events from "~/components/Events.vue";
</script>
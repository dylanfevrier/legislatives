<template>
  <div>
    <Header  />

    <Hero class="px-8 w-full lg:w-[1200px] mx-auto my-10 lg:my-15" />

    <Statement class="px-8 w-full lg:w-[1200px] mx-auto mb-5 lg:mb-10" />

    <Campaign class="mb-5 lg:mb-10"/>

    <div class="px-8 w-full lg:w-[1200px] mx-auto flex flex-col lg:flex-row gap-x-6 gap-y-4 mb-5 lg:mb-10">
      <Applicant class="w-full lg:w-1/2" />
      <Alternate class="w-full lg:w-1/2"/>
    </div>

    <Footer />
  </div>
</template>

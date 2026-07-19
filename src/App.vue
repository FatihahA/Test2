<script setup>
import NavBar from "./components/NavBar.vue";
import Button from "./components/Button.vue";
</script>

<template>
  <section class="w-full h-230 bg-dark-blue">
    <NavBar />
    <h1 class="text-white font-bold text-[4rem] text-center mt-[5rem]">
      Communicate and <br />
      Collaborate <span class="text-med-blue">Seamlessly</span>
    </h1>
    <p class="text-white text-[1.25rem] text-center my-[1.5rem]">
      Ration is a messaging and collaboration platform that offers intuitive,
      flexible and <br />extensible features.
    </p>
    <div class="flex justify-center gap-[0.75rem] my-[1.5rem]">
      <Button> Request Demo </Button>
      <Button class="bg-transparent"> Learn More </Button>
    </div>
    <img src="/HeroImage1.png" class="w-[61.25rem] mx-auto" />
  </section>
  <section class="mt-150">
    <h3>Our Trusted Clients</h3>
    <div class="flex">
      <img src="/TrustedClient1.png" alt="Ogun State Government logo" />
      <img src="/TrustedClient2.png" alt="Nigerian Army logo" />
    </div>
  </section>
</template>

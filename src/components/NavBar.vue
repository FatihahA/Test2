<script setup>
import Button from "./Button.vue";
</script>

<template>
  <section class="flex w-full py-[3rem] px-[5rem] justify-between items-center">
    <img
      class="w-[7.5rem] h-[2.1rem]"
      src="/RationLogo.png"
      alt="Ration logo"
    />
    <ul class="text-white flex items-center gap-[2.5rem] font-medium text-base">
      <li>Home</li>
      <li>Features</li>
      <li>Pricing</li>
      <li>Docs</li>
      <li>Contact</li>
    </ul>
    <Button>Get Started</Button>
  </section>
</template>

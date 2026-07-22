<script setup>
import { ref } from "vue";
import Button from "./Button.vue";

const navItems = ["Home", "Features", "Pricing", "Docs", "Contact"];
const selectedNav = ref("Home");
</script>

<template>
  <section class="flex w-full py-[3rem] px-[5rem] justify-between items-center">
    <img
      class="w-[7.5rem] h-[2.1rem]"
      src="/RationLogo.png"
      alt="Ration logo"
    />
    <ul class="text-white flex items-center gap-[2.5rem] font-medium text-base">
      <li
        v-for="item in navItems"
        :key="item"
        @click="selectedNav = item"
        :class="{
          'border-b-2 border-white pb-[0.15rem]': item === selectedNav,
        }"
      >
        {{ item }}
      </li>
    </ul>
    <Button>Get Started</Button>
  </section>
</template>

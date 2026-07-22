<script setup>
import { ref } from "vue";
import Button from "./Button.vue";

const navItems = ["Home", "Features", "Pricing", "Docs", "Contact"];
const selectedNav = ref("Home");
</script>

<template>
  <section
    class="flex w-full flex-wrap items-center justify-between gap-[1.5rem] px-[1.5rem] py-[1.5rem] md:px-[3rem] md:py-[2rem] lg:px-[5rem] lg:py-[3rem]"
  >
    <img
      class="w-[7.5rem] h-[2.1rem]"
      src="/RationLogo.png"
      alt="Ration logo"
    />
    <ul
      class="order-3 flex w-full items-center justify-center gap-[1.25rem] overflow-x-auto text-base font-medium text-white md:order-none md:w-auto md:gap-[2.5rem]"
    >
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

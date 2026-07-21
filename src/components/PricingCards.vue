<template>
  <article v-for="content in FeatureContents" :key="content.id" class="border">
    <img :src="content.icon" />
    <h2>{{ content.heading }}</h2>
    <p>{{ content.paragraph }}</p>
  </article>
</template>

<script setup>
const FeatureContents = [
  {
    id: 1,
    icon: "/PIcon1.png",
    heading: "Meeting Capacity",
    paragraph: "Increase concurrent meetings & participant limits",
  },

  {
    id: 2,
    icon: "/PIcon2.png",
    heading: "Recording",
    paragraph: "Meeting recording + cloud storage",
  },

  {
    id: 3,
    icon: "/PIcon3.png",
    heading: "Extra Storage",
    paragraph: "Additional Drive or Mailbox storage",
  },
];
</script>

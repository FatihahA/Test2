<template>
  <article
    v-for="content in FeatureContents"
    :key="content.id"
    class="border-e7-grey rounded-lg w-[22.37rem] bg-white border"
  >
    <div class="p-[1.5rem]">
      <img
        class="bg-xlight-blue rounded-xl w-[3.5rem] h-[3.5rem] p-[0.875rem]"
        :src="content.icon"
      />
      <h2>{{ content.heading }}</h2>
      <p>{{ content.paragraph }}</p>
    </div>
  </article>
</template>

<script setup>
const FeatureContents = [
  {
    id: 1,
    icon: "/Icon1.png",
    heading: "Friendly UI",
    paragraph:
      "Designed with simplicity in mind from ground-up for easy adoption",
  },

  {
    id: 2,
    icon: "/Icon2.png",
    heading: "Flexible Pricing",
    paragraph: "Choose from a variety of pricing plans that fit your budget.",
  },

  {
    id: 3,
    icon: "/Icon3.png",
    heading: "Scalable Platform",
    paragraph:
      "Expand your infrastructure to cater for a growing number of users",
  },

  {
    id: 4,
    icon: "/Icon4.png",
    heading: "24/7 Support",
    paragraph: "Dedicated support team available around the clock to assist",
  },
];
</script>

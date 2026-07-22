<template>
  <section class="grid grid-cols-3">
  <article v-for="content in FeatureContents" :key="content.id" class="m-[2rem] p-[1.5rem] bg-white w-[27rem] rounded-lg">
    <div>
    <img :src="content.icon" class="bg-xlight-blue rounded-xl w-[3rem] h-[3rem] p-[0.875rem]"/>
    <h2 class="font-bold text-[1.75rem] mt-[1.5rem]">{{ content.heading }}</h2>
    <p class="font-base text-text-grey text-[1.125rem] mt-[0.75rem]">{{ content.paragraph }}</p>
    </div>
    <div v-if="content.id===1" class="flex gap-[1rem] items-center mt-[1rem]">
      <p class="text-med-blue font-semibold text-[1.125rem]">Contact sales</p>
      <img src="/ArrowIcon.png" class="w-[1.5rem] h-[1.5rem]">
    </div>

  <div v-if="content.id===2" class="mt-[2.5rem]">
    <p class="font-medium text-[1.125rem]">N500 / 10GB / month</p>
  </div>

  <div v-if="content.id===3" class="mt-[2.5rem]">
    <p class="font-medium text-[1.125rem]">N300 / 10GB / month</p>
  </div>
  </article>
  </section>
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

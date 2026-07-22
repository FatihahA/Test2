<template>
  <section class="flex flex-wrap justify-center gap-[1.5rem]">
    <article
      v-for="content in FeatureContents"
      :key="content.id"
      class="flex w-full max-w-[27rem] flex-col justify-between rounded-lg bg-white p-[1.5rem]"
    >
      <div>
        <img
          :src="content.icon"
          class="bg-xlight-blue rounded-xl w-[3rem] h-[3rem] p-[0.875rem]"
        />
        <h2 class="font-bold text-[1.75rem] mt-[1.5rem]">
          {{ content.heading }}
        </h2>
        <p class="mt-[0.75rem] text-[1.125rem] text-text-grey">
          {{ content.paragraph }}
        </p>
      </div>
      <div
        v-if="content.id === 1"
        class="flex gap-[1rem] items-center mt-[1rem]"
      >
        <p class="text-med-blue font-semibold text-[1.125rem]">Contact sales</p>
        <img src="/ArrowIcon.png" class="w-[1.5rem] h-[1.5rem]" />
      </div>

      <div v-if="content.id === 2" class="mt-[2.5rem]">
        <p class="font-medium text-[1.125rem]">N500 / 10GB / month</p>
      </div>

      <div v-if="content.id === 3" class="mt-[2.5rem]">
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

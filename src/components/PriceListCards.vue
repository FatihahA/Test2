<template>
  <div class="flex gap-[1.5rem] mt-[3rem]">
    <article
      v-for="Plan in DeploymentPlans"
      :key="Plan.id"
      class="bg-white p-[1.5rem] rounded-2xl flex-1 gap-[2rem] h-[42rem] w-[23rem]"
    >
      <h6 class="font-semibold text-[1rem]">{{ Plan.Tier }}</h6>
      <h4 class="font-semibold text-[2.375rem]">{{ Plan.TierName }}</h4>
      <p class="font-medium text-61-grey text-[2.37rem]">
        <span class="font-bold text-[2.5rem] text-black">{{ Plan.Price }}</span
        >/user /year
      </p>
      <p>Billed Annually</p>
      <p>{{ Plan.description }}</p>
      <div
        class="flex gap-[1rem]"
        v-for="feature in Plan.features"
        :key="feature"
      >
        <img class="w-[1.5rem] h-[1.5rem]" src="/CheckIcon.png" />
        <p>{{ feature }}</p>
        <p></p>
      </div>
      <Button>{{ Plan.ButtonText }}</Button>
    </article>
  </div>
</template>

<script setup>
import Button from "./Button.vue";

const DeploymentPlans = [
  {
    id: 1,
    Tier: "ENTRY",
    TierName: "Ration Start",
    Price: "N2,000",
    description: "Secure communication foundation",
    features: [
      "Mail (25GB per user)",
      "Calendar",
      "Basic Chat",
      "Mobile + Desktop apps",
      "MFA / Identity",
    ],
    ButtonText: "Start with collaboration",
  },

  {
    id: 2,
    Tier: "REVENUE ENGINE",
    TierName: "Ration Do",
    Price: "N4,000",
    description: "Where teams actually work together",
    features: [
      "Everything in Start, plus:",
      "Rooms (video/audio meetings)",
      "Full Chat + Channels",
      "Drive & File sharing",
      "Notes / Wiki",
      "Workflow / Approvals",
    ],
    ButtonText: "Do the work",
  },

  {
    id: 3,
    Tier: "ENTERPRISE",
    TierName: "Ration Scale",
    Price: "N6,000",
    description: "Control, compliance, scale",
    features: [
      "Everything in Do, plus:",
      "Audit logs",
      "Compliance controls",
      "Policy enforcement",
      "Priority support",
      "Higher usage limits",
    ],
    ButtonText: "Scale with confidence",
  },
];
</script>

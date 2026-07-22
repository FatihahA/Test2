<template>
  <div class="mt-[3rem] flex flex-wrap justify-center gap-[1.5rem]">
    <article
      v-for="Plan in PricePlans"
      :key="Plan.id"
      :class="['flex w-full max-w-[23rem] flex-col rounded-2xl bg-white p-[1.5rem] shadow-md', Plan.id===2?'border border-2 border-[#00669933]':'border-none']"
    >
      <div class="space-y-[0.75rem]">
        <h6 :class="Plan.TierClass">{{ Plan.Tier }}</h6>
        <h4 class="text-[2.375rem] mt-[1rem] font-semibold leading-tight">{{ Plan.TierName }}</h4>
        <p class="text-[1.125rem] font-medium text-61-grey">
          <span class="text-[2.5rem] font-bold text-black">{{ Plan.Price }}</span>
          /user /year
        </p>
        <p class="text-[0.95rem] text-61-grey">Billed Annually</p>
        <p class="text-[0.95rem] leading-6 text-61-grey">{{ Plan.description }}</p>
      </div>

      <div class="mt-[1.5rem] flex flex-col gap-[0.875rem]">
        <div
          v-for="feature in Plan.features"
          :key="feature"
          class="flex items-start gap-[0.75rem]"
        >
          <img class="mt-[0.2rem] h-[1.25rem] w-[1.25rem] shrink-0" src="/CheckIcon.png" />
          <p class="text-[0.95rem] leading-6 text-text-grey">{{ feature }}</p>
        </div>
      </div>
        <hr v-if="Plan.id === 1" class="border-t border-e7-grey mt-[0.5rem]" />

      <div v-if="Plan.id===1" class="gap-[1rem] mt-[0.5rem]">
        <div class="flex gap-[1rem] items-center">
         <img src="/DotIcon.png" class="w-[0.5rem] h-[0.5rem]" />
        <p class="font-base text-[0.875rem] text-text-grey">Rooms (video/audio)</p>
        </div>
        <div class="flex gap-[1rem] items-center">
        <img src="/DotIcon.png" class="w-[0.5rem] h-[0.5rem]" />
        <p class="font-base text-[0.875rem] text-text-grey">Drive / Notes / Workflows</p>
       </div>
      </div>

      <div v-if="Plan.id===2">
        <div class="flex gap-[1rem] bg-[#F8FBFC] p-[0.3rem] mt-[0.5rem]">
          <img src="/BlueInfoIcon.png" class="w-[1.5rem] h-[1.5rem]"/>
          <p>60-min meetings · 25 participants · Fair usage limits apply</p>
        </div>
      </div>

      <div v-if="Plan.id===3">
        <div class="flex gap-[1rem] bg-[#F8FBFC] p-[0.3rem] mt-[0.5rem]">
          <img src="/GreyInfoIcon.png" class="w-[1.5rem] h-[1.5rem]" />
          <p class="text-text-grey">120-min meetings · 50 participants · Higher concurrency</p>
        </div>
      </div>


      <Button :class="Plan.ButtonClass">{{ Plan.ButtonText }}</Button>
    </article>
  </div>
</template>

<script setup>
import Button from "./Button.vue";

const PricePlans = [
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
    TierClass:"text-[1rem] inline font-semibold bg-[#f4f4f4] rounded-full p-[0.7rem]",
    ButtonClass: "mt-[2rem] w-full  border border-e7-grey text-black bg-white",
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
    TierClass:"text-[1rem] text-med-blue inline font-semibold bg-[#f5f9fb] rounded-full p-[0.7rem]",
    ButtonClass: "mt-[2rem] w-full bg-[#006699]",
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
    TierClass:"text-[1rem] inline text-white font-semibold bg-black rounded-full p-[0.7rem]",
    ButtonClass: "mt-[2rem] w-full border border-e7-grey text-black bg-white",
  },
];
</script>

<template>
  <section class="bg-bckg-blue py-[5rem] px-[2rem]">
  <h3 class="font-bold text-black text-[3.5rem] text-center">Deployment Plan</h3>
    <p class="font-base text-61-grey text-center text-[1rem]">
      Choose the deployment edition that best aligns with your organization's<br />
      requirements, resources, and strategic objectives.
    </p>
  <div class="mt-[3rem] grid grid-cols-1 justify-items-center gap-[1.5rem] md:grid-cols-2 lg:grid-cols-3">
  <article
    v-for="plan in DeploymentPlans"
    :key="plan.id"
    class="flex w-full max-w-[24rem] flex-col justify-between rounded-2xl bg-white p-[1.5rem] shadow-sm"
  >
    <div>
      <h4 class="font-bold text-[1.125rem] text-center whitespace-pre-line mb-[1.5rem]">{{ plan.heading }}</h4>
      <p class="font-base text-[1rem] whitespace-pre-line text-text-grey text-center mb-[2rem]">{{ plan.description }}</p>
      <div class="flex flex-col gap-[1.5rem]">
        <div
          class="flex gap-[1rem]"
          v-for="feature in plan.features"
          :key="feature"
        >
          <img class="w-[1.5rem] h-[1.5rem]" src="/CheckIcon.png" />
          <p>{{ feature }}</p>
        </div>
      </div>
    </div>
    <Button class="mt-[3rem] w-full"
    v-if="id===1">Get Started</Button>
  </article>
  </div>
  </section>
</template>

<script setup>
import Button from "./Button.vue";

const DeploymentPlans = [
  {
    id: 1,
    heading: "Software-As-A-Service \n(SaaS) Edition",
    description:
      "Cloud-Based Service: Hosted and managed and maintained by our expert team",
    features: [
      "Cloud-Based Service: Hosted and managed by Ration's expert team",
      "Subscription-Based: Flexible subscription plans to fit different business sizes and needs.",
      "Automatic Updates: Always have access to the latest features and security patches",
      "Scalability: Easily scale up or down as your business needs change",
    ],
  },

  {
    id: 2,
    heading: "Managed Service \nProvider (MSP) Edition",
    description:
      "Host within your environment and extend your \nservice offerings",
    features: [
      "Cloud-Based Service: Hosted and managed by Ration's expert team",
      "Multi-Tenancy Support: Support hosting different customers within the same infrastructure",
      "Unlimited Scaling: Vertically scale your infrastructure to handle more tenants",
      "Premium support: Enjoy priority support from our development team to customize your platform",
    ],
  },

  {
    id: 3,
    heading: "Data Center (DC) On-\nPremise Edition",
    description:
      "Deploy within your Data Center for maximum \ncontrol and security",
    features: [
      "Your Own Data Center: Deployed directly onto your hardware or IaaS",
      "Maximum Control: Complete ownership and control over your deployment environment",
      "Enhanced Security: Leverage your existing security protocols and measures",
      "Customization: Tailor the deployment to fit your specific business needs",
    ],
  },
];
</script>

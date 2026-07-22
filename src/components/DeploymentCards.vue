<template>
  <section
    class="bg-bckg-blue px-[1.5rem] py-[5rem] md:px-[3rem] lg:px-[5rem] lg:py-[7.5rem]"
  >
    <h3
      class="text-center text-[2.5rem] font-bold leading-tight text-black md:text-[3.5rem]"
    >
      Deployment Plan
    </h3>
    <p
      class="mx-auto mt-[0.75rem] max-w-[48rem] text-center text-[1rem] text-61-grey"
    >
      Choose the deployment edition that best aligns with your organization's<br
        class="hidden md:block"
      />
      requirements, resources, and strategic objectives.
    </p>
    <div class="mt-[3rem] flex flex-wrap justify-center gap-[1.5rem]">
      <article
        v-for="plan in DeploymentPlans"
        :key="plan.id"
        class="flex w-full max-w-[24rem] flex-col justify-between rounded-2xl bg-white p-[1.5rem] shadow-sm"
      >
        <div>
          <h4
            class="font-bold text-[1.125rem] text-center whitespace-pre-line mb-[1.5rem]"
          >
            {{ plan.heading }}
          </h4>
          <p
            class="mb-[2rem] whitespace-pre-line text-center text-[1rem] text-text-grey"
          >
            {{ plan.description }}
          </p>
          <div class="flex flex-col gap-[1.5rem]">
            <div
              class="flex gap-[1rem]"
              v-for="feature in plan.features"
              :key="feature"
            >
              <img
                class="h-[1.5rem] w-[1.5rem] shrink-0"
                src="/CheckIcon.png"
              />
              <p>{{ feature }}</p>
            </div>
          </div>
        </div>
        <Button class="mt-[3rem] w-full">Get Started</Button>
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

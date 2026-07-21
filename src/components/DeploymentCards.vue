<template>
  <article v-for="plan in DeploymentPlans" :key="plan.id">
    <h4>{{ plan.heading }}</h4>
    <p>{{ plan.description }}</p>
    <div>
      <div v-for="feature in plan.features" :key="feature">
        <img src="/CheckIcon.png" />
        <p>{{ feature }}</p>
      </div>
      <Button>Get Started</Button>
    </div>
  </article>
</template>

<script setup>
import Button from "./Button.vue";

const DeploymentPlans = [
  {
    id: 1,
    heading: "Software-As-A-Service (SaaS) Edition",
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
    heading: "Managed Service Provider (MSP) Edition",
    description:
      "Host within your environment and extend your service offerings",
    features: [
      "Cloud-Based Service: Hosted and managed by Ration's expert team",
      "Multi-Tenancy Support: Support hosting different customers within the same infrastructure",
      "Unlimited Scaling: Vertically scale your infrastructure to handle more tenants",
      "Premium support: Enjoy priority support from our development team to customize your platform",
    ],
  },

  {
    id: 3,
    heading: "Data Center (DC) On-Premise Edition",
    description:
      "Deploy within your Data Center for maximum control and security",
    features: [
      "Your Own Data Center: Deployed directly onto your hardware or IaaS",
      "Maximum Control: Complete ownership and control over your deployment environment",
      "Enhanced Security: Leverage your existing security protocols and measures",
      "Customization: Tailor the deployment to fit your specific business needs",
    ],
  },
];
</script>

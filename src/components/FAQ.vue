<template>
  <section
    class="bg-white px-[1.5rem] py-[5rem] md:px-[3rem] lg:px-[5rem] lg:py-[7.5rem]"
  >
    <h3
      class="mb-[1rem] text-center text-[2.5rem] font-bold leading-tight md:text-[3.5rem]"
    >
      Frequently Asked Questions
    </h3>
    <article>
      <div
        class="flex items-start gap-[1.5rem] bg-[#f8f8f8] px-[1rem] py-[1rem] md:items-center"
      >
        <div class="flex-1">
          <h3 class="text-med-blue font-bold text-[1rem]">
            How secure is Ration?
          </h3>
          <p class="text-[1rem]">
            Security is our top priority. Ration employs robust security
            measures to protect your data, including encryption, authentication,
            and regular security audits. We <br />adhere to industry-leading
            standards to ensure the confidentiality, integrity, and availability
            of your information.
          </p>
        </div>
        <img class="h-[2rem] w-[2rem] shrink-0" src="/MinusIcon.png" />
      </div>
    </article>
    <article
      v-for="faq in faqs"
      :key="faq"
      class="mb-[0.5rem] flex items-center justify-between gap-[1rem] border-b border-[#f8f8f8] px-[1rem] py-[1rem]"
    >
      <h4 class="text-[1.125rem] font-semibold md:text-[1.25rem]">{{ faq }}</h4>
      <img src="/PlusIcon.png" class="h-[2rem] w-[2rem] shrink-0" />
    </article>
  </section>
</template>

<script setup>
const faqs = [
  "What kind of support does Ration offer?",
  "Can I control user access and permissions in Ration?",
  "Can I migrate my data from another platform to Ration?",
];
</script>

<template>
  <section class="bg-white px-[5rem] py-[7.5rem]">
    <h3 class="font-bold text-[3.5rem] text-center mb-[1rem]">
      Frequently Asked Questions
    </h3>
    <article>
      <div
        class="gap-[1.5rem] items-center bg-[#f8f8f8] flex px-[0.5rem] py-[1rem]"
      >
        <div class="flex-1">
          <h3 class="text-med-blue font-bold text-[1rem]">
            How secure is Ration?
          </h3>
          <p class="text-base text-[1rem]">
            Security is our top priority. Ration employs robust security
            measures to protect your data, including encryption, authentication,
            and regular security audits. We <br />adhere to industry-leading
            standards to ensure the confidentiality, integrity, and availability
            of your information.
          </p>
        </div>
        <img class="w-[2rem] h-[2rem]" src="/MinusIcon.png" />
      </div>
    </article>
    <article
      v-for="faq in faqs"
      :key="faq"
      class="flex items-center gap-[0.5rem] mb-[0.5rem] justify-between border-b border-[#f8f8f8] px-[0.5rem] py-[1rem]"
    >
      <h class="font-semibold text-[1.25rem]">{{ faq }}</h>
      <img src="/PlusIcon.png" class="w-[2rem] h-[2rem]" />
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

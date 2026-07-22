<script setup>
import NavBar from "./components/NavBar.vue";
import Button from "./components/Button.vue";
import SlideCard from "./components/SlideCard.vue";
import FeatureCards from "./components/FeatureCards.vue";
import PricingCards from "./components/PricingCards.vue";
import Footer from "./components/Footer.vue";
import BetaTesting from "./components/BetaTesting.vue";
import FAQ from "./components/FAQ.vue";
import DeploymentCards from "./components/DeploymentCards.vue";
import PriceListCards from "./components/PriceListCards.vue";
</script>

<template>
  <section class="w-full bg-dark-blue lg:h-230">
    <NavBar />
    <h1
      class="mx-auto mt-[3rem] max-w-[56rem] px-[1.5rem] text-center text-[2.5rem] font-bold leading-tight text-white md:mt-[5rem] md:text-[4rem]"
    >
      Communicate and <br />
      Collaborate <span class="text-med-blue">Seamlessly</span>
    </h1>
    <p
      class="mx-auto my-[1.5rem] px-[1.5rem] text-center text-[1.125rem] text-white md:text-[1.25rem]"
    >
      Ration is a messaging and collaboration platform that offers intuitive,
      flexible and <br />extensible features.
    </p>
    <div
      class="my-[1.5rem] flex flex-wrap justify-center gap-[0.75rem] px-[1.5rem]"
    >
      <Button> Request Demo </Button>
      <Button class="bg-transparent"> Learn More </Button>
    </div>
    <img
      src="/HeroImage1.png"
      class="mx-auto w-full max-w-[61.25rem] px-[1.5rem] lg:w-[61.25rem] lg:px-0"
    />
  </section>
  <section
    class="relative mt-[4rem] flex justify-center px-[1.5rem] py-[4rem] lg:mt-120 lg:py-0"
  >
    <div>
      <h3 class="text-base text-[1.5rem] text-center">Our Trusted Clients</h3>
      <div class="flex gap-[1.821rem] justify-center pb-[2rem]">
        <img
          src="/TrustedClient1.png"
          class="h-[4.25rem] w-[4.25rem]"
          alt="Ogun State Government logo"
        />
        <img
          src="/TrustedClient2.png"
          class="w-[4.25rem] h-[4.25rem]"
          alt="Nigerian Army logo"
        />
      </div>
    </div>
    <button
      aria-label="Open chat"
      class="absolute bottom-[1.5rem] right-[1.5rem] md:bottom-[2rem] md:right-[2rem] h-[3.5rem] w-[3.5rem] p-0 flex items-center justify-center rounded-full bg-med-blue shadow-lg z-10"
    >
      <img
        src="/SidechatIcon.png"
        alt="side chat"
        class="h-[1.75rem] w-[1.75rem] object-contain"
      />
    </button>
  </section>
  <section
    class="bg-off-white px-[1.5rem] py-[5rem] md:px-[3rem] lg:px-[5rem] lg:py-[7.5rem]"
  >
    <h2
      class="text-center text-[2.5rem] font-bold leading-tight md:text-[3.5rem]"
    >
      Messaging. Meetings. <br class="hidden sm:block" />collaboration.
    </h2>
    <p class="mx-auto mt-[1.5rem] text-center text-[1.125rem]">
      Aside providing the whole gamut for email messaging - SMTP, IMAP, POP3 and
      friends - we are <br />focussed on extending your collaboration needs with
      more productive apps.
    </p>
    <section class="mt-[2rem] flex items-center justify-center gap-[1.5rem]">
      <button
        class="hidden h-[3rem] w-[3rem] shrink-0 items-center justify-center rounded-full bg-[#f4f4f4] md:flex"
      >
        <img
          src="/BlackArrowIcon.png"
          class="h-[1.5rem] w-[1.5rem] object-contain"
          alt="arrow left"
        />
      </button>
      <div class="shrink-0 w-[61.25rem]">
        <SlideCard />
      </div>
      <button
        class="hidden h-[3rem] w-[3rem] shrink-0 items-center justify-center rounded-full bg-[#f4f4f4] md:flex"
      >
        <img
          src="/BlackArrowIcon2.png"
          class="h-[1.5rem] w-[1.5rem] object-contain"
          alt="arrow right"
        />
      </button>
    </section>
  </section>

  <section
    class="grid gap-[3rem] bg-white px-[1.5rem] py-[5rem] md:px-[3rem] lg:grid-cols-[31.375rem_1fr] lg:gap-[4rem] lg:px-[5rem] lg:py-[7.5rem]"
  >
    <div>
      <h4 class="font-medium text-[1.25rem] text-med-blue">
        Why Choose Ration
      </h4>
      <h2
        class="mt-[0.5rem] text-[2.25rem] font-bold leading-tight md:text-[3rem] md:leading-none"
      >
        Easily extendable. Thoughtful UI/UX. Flexible Pricing.
      </h2>
      <p class="text-base text-[1.125rem] mt-[3rem] text-text-grey">
        Smart APIs, seamless experiences, and open-source value, keeping
        innovation simple and costs low.
      </p>
      <Button class="mt-[3rem]">Get Started</Button>
    </div>
    <div
      class="grid w-full grid-cols-1 gap-[1.5rem] justify-self-center sm:grid-cols-2 lg:w-fit"
    >
      <FeatureCards />
    </div>
  </section>
  <section
    class="bg-off-white px-[1.5rem] py-[5rem] md:px-[3rem] lg:px-[5rem] lg:py-[7.5rem]"
  >
    <h2
      class="text-center text-[2.5rem] font-bold leading-tight md:text-[3.5rem]"
    >
      Pricing Plans
    </h2>
    <p class="mt-[0.625rem] text-center text-[1.125rem] md:text-[1.25rem]">
      Start with collaboration. Do the work. Scale with confidence.
    </p>
    <div
      class="mt-[0.5rem] flex flex-wrap items-center justify-center gap-[1rem]"
    >
      <p class="text-[1rem] text-text-grey">Select your currency:</p>
      <div
        class="flex w-full max-w-[14.25rem] items-center justify-between gap-x-[1rem] rounded-md border border-e7-grey px-[1rem] py-[0.5rem]"
      >
        <p>NGN - Nigeria Naira</p>
        <img class="w-[1.125rem] h-[1.125rem]" src="/DropdownIcon.png" />
      </div>
    </div>
    <div class="flex items-center justify-center mt-[3rem]">
      <div
        class="grid w-full max-w-[21.2rem] grid-cols-[7rem_1fr] items-center overflow-hidden rounded-full bg-white"
      >
        <p
          class="bg-dark-blue rounded-full text-white w-full py-[0.75rem] text-center"
        >
          Monthly
        </p>
        <p class="py-[0.75rem] text-center">Annual (save 2 months)</p>
      </div>
    </div>
    <PriceListCards />
    <p
      class="mx-auto mt-[2rem] max-w-[70rem] text-center text-[1rem] text-text-grey md:text-[1.125rem]"
    >
      All prices exclude VAT where applicable. Annual plans billed upfront.
      Savings calculated against monthly pricing. Fair usage limits apply to
      Ration Do and Ration Scale. 24/7 email support for all tiers. Priority
      support for Ration Scale.
    </p>
    <h3
      class="my-[1.5rem] text-center text-[2rem] font-semibold leading-tight md:text-[2.5rem]"
    >
      Need more? Add what you need.
    </h3>
    <PricingCards />
  </section>
  <section>
    <DeploymentCards />
  </section>
  <section>
    <FAQ />
  </section>
  <section>
    <BetaTesting />
  </section>
  <section>
    <Footer />
  </section>
</template>

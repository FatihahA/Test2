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
  <section class="w-full h-230 bg-dark-blue">
    <NavBar />
    <h1 class="text-white font-bold text-[4rem] text-center mt-[5rem]">
      Communicate and <br />
      Collaborate <span class="text-med-blue">Seamlessly</span>
    </h1>
    <p class="text-white text-[1.25rem] text-center my-[1.5rem]">
      Ration is a messaging and collaboration platform that offers intuitive,
      flexible and <br />extensible features.
    </p>
    <div class="flex justify-center gap-[0.75rem] my-[1.5rem]">
      <Button> Request Demo </Button>
      <Button class="bg-transparent"> Learn More </Button>
    </div>
    <img src="/HeroImage1.png" class="w-[61.25rem] mx-auto" />
  </section>
  <section class="mt-120 flex justify-center">
    <div>
      <h3 class="text-base text-[1.5rem] text-center">Our Trusted Clients</h3>
      <div class="flex gap-[1.821rem] justify-center pb-[2rem]">
        <img
          src="/TrustedClient1.png"
          class="w-[3.946rem] w-[3.946rem]"
          alt="Ogun State Government logo"
        />
        <img
          src="/TrustedClient2.png"
          class="w-[4.25rem] h-[4.25rem]"
          alt="Nigerian Army logo"
        />
      </div>
    </div>
  </section>
  <section class="bg-off-white px-[5rem] py-[7.5rem]">
    <h2 class="font-bold text-[3.5rem] text-center">
      Messaging. Meetings. <br />collaboration.
    </h2>
    <p class="mt-[1.5rem] text-base text-center text-[1.25rem]">
      Aside providing the whole gamut for email messaging - SMTP, IMAP, POP3 and
      friends - we are <br />focussed on extending your collaboration needs with
      more productive apps.
    </p>
    <section class="flex items-center">
      <button class="flex h-[3rem] w-[3rem] items-center justify-center rounded-full bg-[#f4f4f4]">
        <img
          src="/BlackArrowIcon.png"
          class="h-[1.5rem] w-[1.5rem] object-contain"
          alt="arrow left"
        />
      </button>
      <SlideCard />
      <button class="flex h-[3rem] w-[3rem] items-center justify-center rounded-full bg-[#f4f4f4]">
        <img
          src="/BlackArrowIcon2.png"
          class="h-[1.5rem] w-[1.5rem] object-contain"
          alt="arrow right"
        />
      </button>
    </section>
  </section>

  <section
    class="bg-white py-[7.5rem] px-[5rem] grid grid-cols-[31.375rem_1fr] gap-[4rem]"
  >
    <div>
      <h4 class="font-medium text-[1.25rem] text-med-blue">
        Why Choose Ration
      </h4>
      <h2 class="font-bold text-[3rem] leading-none mt-[0.5rem]">
        Easily extendable. Thoughtful UI/UX. Flexible Pricing.
      </h2>
      <p class="text-base text-[1.125rem] mt-[3rem] text-text-grey">
        Smart APIs, seamless experiences, and open-source value, keeping
        innovation simple and costs low.
      </p>
      <Button class="mt-[3rem]">Get Started</Button>
    </div>
    <div class="grid grid-cols-2 gap-[1.5rem] justify-self-center w-fit">
      <FeatureCards />
    </div>
  </section>
  <section class="bg-off-white py-[7.5rem] px-[5rem]">
    <h2 class="font-bold text-[3.5rem] text-center">Pricing Plans</h2>
    <p class="text-base text-[1.25rem] text-center mt-[0.625rem]">
      Start with collaboration. Do the work. Scale with confidence.
    </p>
    <div class="flex gap-[1rem] items-center mt-[0.5rem] justify-center">
      <p class="text-[1rem] text-text-grey">Select your currency:</p>
      <div
        class="flex items-center gap-x-[1rem] w-[14.25rem] py-[0.5rem] px-[1rem] border border-e7-grey rounded-md"
      >
        <p>NGN - Nigeria Naira</p>
        <img class="w-[1.125rem] h-[1.125rem]" src="/DropdownIcon.png" />
      </div>
    </div>
    <div class="flex items-center justify-center mt-[3rem]">
      <div
        class="bg-white rounded-full grid grid-cols-[7rem_1fr] items-center w-[21.2rem] overflow-hidden"
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
    <p class="font-base text-[1.125rem] text-center text-text-grey mt-[2rem]">
      All prices exclude VAT where applicable. Annual plans billed upfront.
      Savings calculated against monthly pricing. Fair usage limits apply to
      Ration Do and Ration Scale. 24/7 email support for all tiers. Priority
      support for Ration Scale.
    </p>
    <h3 class="font-lg text-[2.5rem] text-center my-[1.5rem]">Need more? Add what you need.</h3>
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

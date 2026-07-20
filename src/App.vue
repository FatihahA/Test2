<script setup>
import NavBar from "./components/NavBar.vue";
import Button from "./components/Button.vue";
import SlideCard from "./components/SlideCard.vue";
import FeatureCards from "./components/FeatureCards.vue"
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
      <div class="flex gap-[1.821rem] justify-center">
      <img src="/TrustedClient1.png" class="w-[3.946rem] w-[3.946rem]" alt="Ogun State Government logo" />
      <img src="/TrustedClient2.png" class="w-[4.25rem] h-[4.25rem]" alt="Nigerian Army logo" />
    </div>
    </div>
  </section>
  <section class="bg-off-white px-[5rem] py-[7.5rem]">
    <h2>Messaging. Meetings. collaboration.</h2>
    <p>Aside providing the whole gamut for email messaging - SMTP, IMAP, POP3 and friends 
      - we are focussed on extending your collaboration needs with more productive apps.</p>
    <SlideCard />
    
  </section>

  <section>
    <div>
      <h4>Why Choose Ration</h4>
      <h2>Easily extendable. Thoughtful UI/UX. Flexible Pricing.</h2>
      <p>Smart APIs, seamless experiences, and open-source value,
         keeping innovation simple and costs low.</p>
      <Button>Get Started</Button>
    </div>
    <FeatureCards />
  </section>
  <section>
    <h2>Pricing Plans</h2>
    <p>Start with collaboration. Do the work. Scale with confidence.</p>
  </section>
</template>
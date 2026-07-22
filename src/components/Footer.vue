<template>
  <footer
    class="bg-white px-[1.5rem] py-[3rem] text-black md:px-[3rem] lg:px-[5rem]"
  >
    <div
      class="flex flex-col justify-between gap-[3rem] lg:flex-row lg:gap-[5rem]"
    >
      <div class="w-full max-w-[25rem]">
        <img
          src="/StackchaseLogo.png"
          class="w-[7.5rem] h-auto"
          alt="Stackchase logo"
        />
        <p
          class="mt-[1rem] text-[1.125rem] leading-[1.5] text-text-grey md:text-[1.25rem]"
        >
          Stackchase Limited is a technology company<br
            class="hidden lg:block"
          />
          building secure, high-performance platforms<br
            class="hidden lg:block"
          />
          that power modern collaboration,<br class="hidden lg:block" />
          communication and digital operations.
        </p>
      </div>

      <nav
        class="grid grid-cols-1 gap-[2rem] text-[1.125rem] sm:grid-cols-3 lg:gap-[5rem] lg:text-[1.25rem]"
      >
        <div>
          <h6 class="font-semibold">Company</h6>
          <ul class="mt-[0.75rem] space-y-[0.5rem] text-text-grey">
            <li>About</li>
            <li>Product</li>
            <li>News</li>
            <li>Career</li>
          </ul>
        </div>

        <div>
          <h6 class="font-semibold">Industry</h6>
          <ul class="mt-[0.75rem] space-y-[0.5rem] text-text-grey">
            <li>Government</li>
            <li>Business</li>
          </ul>
        </div>

        <div>
          <h6 class="font-semibold text-[1.2rem]">Support</h6>
          <ul
            class="mt-[0.75rem] space-y-[0.5rem] text-[1.25rem] text-text-grey"
          >
            <li>Product support</li>
            <li>Contact Us</li>
          </ul>
        </div>
      </nav>
    </div>

    <hr class="border-t border-61-grey mt-[3rem]" />
    <div
      class="flex flex-col justify-between gap-[2rem] text-[1rem] text-text-grey lg:flex-row lg:items-center lg:text-[1.25rem]"
    >
      <div
        class="flex flex-wrap items-center gap-[1rem] pt-[1rem] lg:gap-[2rem]"
      >
        <p>Copyright 2025 Stackchase Limited. All right reserved.</p>
        <p>Privacy policy</p>
        <p>Legal notice</p>
        <p>Feedback</p>
      </div>

      <div class="flex items-center gap-[1rem]">
        <img class="w-[1.5rem] h-[1.5rem]" src="/MailIcon.png" alt="Email" />
        <img
          class="w-[1.5rem] h-[1.5rem]"
          src="/FacebookIcon.png"
          alt="Facebook"
        />
        <img class="w-[1.5rem] h-[1.5rem]" src="/XIcon.png" alt="X" />
        <img
          class="w-[1.5rem] h-[1.5rem]"
          src="/LinkedinIcon.png"
          alt="LinkedIn"
        />
        <img
          class="w-[1.5rem] h-[1.5rem]"
          src="/InstagramIcon.png"
          alt="Instagram"
        />
      </div>
    </div>
  </footer>
</template>

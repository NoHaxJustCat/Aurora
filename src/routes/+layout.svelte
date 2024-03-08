<script>
  import {
    NavBrand,
    NavHamburger,
    NavLi,
    NavUl,
    Navbar,
  } from "flowbite-svelte";
  import "../app.css";
  import {
    Footer,
    FooterCopyright,
    FooterLinkGroup,
    FooterBrand,
    FooterLink,
  } from "flowbite-svelte";
</script>

<Navbar class="border-b border-white">
  <NavBrand href="/">
    <img
      src="/AuroraLogo.svg"
      class="me-3 h-8 sm:h-12 hover:fill-primary-700"
      alt="Aurora Logo"
    />
    <span class="self-center whitespace-nowrap text-xl font-semibold"
      >Aurora</span
    >
  </NavBrand>

  <NavHamburger />

  <NavUl>
    <NavLi href="/">Home</NavLi>
    <NavLi href="/team">The Team</NavLi>
    <NavLi href="/contact">Contact</NavLi>
  </NavUl>
</Navbar>

<slot />

<footer class="bg-[#111827]">
  <div class="mx-auto w-full max-w-screen-xl p-4 py-6 lg:py-8">
    <div class="md:flex md:justify-between">
      <div class="mb-6 md:mb-0">
        <a href="https://aurorarocketry.eu/" class="flex items-center">
          <img
            src="/AuroraLogo.svg"
            class="h-8 scale-150 me-3"
            alt="Aurora Logo"
          />
          <span
            class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white"
            >Aurora Rocketry Team</span
          >
        </a>
      </div>
    </div>
    <hr class="my-6 border-gray-200 sm:mx-auto dark:border-gray-700 lg:my-8" />
    <div class="sm:flex sm:items-center sm:justify-between">
      <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400"
        >© 2024 <a href="https://flowbite.com/" class="hover:underline"
          >Aurora Rocketry Team</a
        >. All Rights Reserved.
      </span>
      <div class="flex mt-4 sm:justify-center sm:mt-0"></div>
    </div>
  </div>
</footer>

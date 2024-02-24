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
      src="/static/AuroraLogo.svg"
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
    <NavLi href="/theteam">The Team</NavLi>
    <NavLi href="/contact">Contact</NavLi>
  </NavUl>
</Navbar>

<slot />
<Footer footerType="logo" class=" dark:bg-[#111827] rounded-none z-30">
  <div
    class=" sm:flex sm:items-center sm:justify-between bottom-0 mt-auto"
  ></div>
  <hr class="my-6 border-gray-200 sm:mx-auto dark:border-gray-700 lg:my-8" />
  <FooterCopyright href="/" by="Flowbite™" />
</Footer>

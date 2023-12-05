<script>
  import { Navbar, NavBrand, NavHamburger, NavUl, NavLi, Footer, FooterCopyright, FooterLink, FooterLinkGroup } from "flowbite-svelte";
  import "../app.pcss";
</script>

<Navbar class="bg-red-600">
  <NavBrand href="/">
    <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">Flowbite</span>
  </NavBrand>
  <NavHamburger  />
  <NavUl >
    <NavLi href="/">Home</NavLi>
    <NavLi href="/about">About</NavLi>
    <NavLi href="/products">Products</NavLi>
  </NavUl>
</Navbar>
<div class="container mx-auto px-4 py-8 bg-gray-600 h-screen">
  <slot />
</div>

<Footer>
  <FooterCopyright href="/" by="Flowbite™" year={2022} />
  <FooterLinkGroup ulClass="flex flex-wrap items-center mt-3 text-sm text-gray-500 dark:text-gray-400 sm:mt-0">
    <FooterLink href="/">About</FooterLink>
    <FooterLink href="/">Privacy Policy</FooterLink>
    <FooterLink href="/">Licensing</FooterLink>
    <FooterLink href="/">Contact</FooterLink>
  </FooterLinkGroup>
</Footer>


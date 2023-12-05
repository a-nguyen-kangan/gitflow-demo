<script>
  import { Navbar, NavBrand, NavHamburger, NavUl, NavLi } from "flowbite-svelte";
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
<div class="container mx-auto px-4 py-8 bg-gray-200 h-screen">
  <slot />
</div>
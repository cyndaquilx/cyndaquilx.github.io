<script lang="ts">
    import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
    import { base } from '$app/paths';

    let activeClass = "";
    let nonActiveClass = "text-white hover:text-gray-300"
</script>

<Navbar class="bg-primary-800 text-white">
  <NavBrand href="{base}/">
    <!-- <img src="/images/flowbite-svelte-icon-logo.svg" class="me-3 h-6 sm:h-9" alt="Flowbite Logo" /> -->
    <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">Cynda's Site</span>
  </NavBrand>
  <NavHamburger  />
  <NavUl {nonActiveClass}>
    <NavLi href="{base}/">Home</NavLi>
    <NavLi href="{base}/test">Test</NavLi>
  </NavUl>
</Navbar>
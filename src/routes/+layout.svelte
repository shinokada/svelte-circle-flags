<script>
  import '../app.postcss';
  import { page } from '$app/stores';
  import DarkMode from 'flowbite-svelte/DarkMode.svelte';
  import Navbar from 'flowbite-svelte/Navbar.svelte';
  import NavBrand from 'flowbite-svelte/NavBrand.svelte';
  import NavLi from 'flowbite-svelte/NavLi.svelte';
  import NavUl from 'flowbite-svelte/NavUl.svelte';
  import NavHamburger from 'flowbite-svelte/NavHamburger.svelte';
  import Footer from 'flowbite-svelte/Footer.svelte'
  import FooterBrand from 'flowbite-svelte/FooterBrand.svelte'
  import FooterLinkGroup from 'flowbite-svelte/FooterLinkGroup.svelte'
  import FooterLink from 'flowbite-svelte/FooterLink.svelte'
  import { MetaTags } from 'svelte-meta-tags';

  $: activeUrl = $page.url.pathname;
</script>

<MetaTags
  title="Svelte Circle Flags"
  description="Circle Flags icon set for Svelte"
  openGraph={{
    type: 'website',
    url: 'https://svelte-circle-flags.vercel.app/',
    title: "Svelte Circle Flags",
    description: "Circle Flags icon set for Svelte",
    images: [{ url: 'https://open-graph-vercel.vercel.app/api/svelte-circle-flags', width: 1200, height: 630, alt: "Svelte Circle Flags Icons" }],
    site_name: 'Svelte Circle Flags'
  }}
  twitter={{
    handle: '@shinokada',
    cardType: 'summary_large_image',
    title: "Svelte Circle Flags",
    description: "Circle Flags icon set for Svelte",
    image:'https://open-graph-vercel.vercel.app/api/svelte-circle-flags',
    imageAlt: "Svelte Circle Flags"
  }} />
  
<Navbar let:hidden let:toggle class="dark:bg-zinc-700" >
  <NavBrand href="/">
    <span class="self-center whitespace-nowrap text-2xl font-semibold text-primary-700 dark:text-primary-500">
      Svelte Circle Flags
    </span>
  </NavBrand>
  <NavHamburger on:click={toggle} />
  <NavUl {hidden}>
    <NavLi href="/" active={activeUrl === '/'}>Home</NavLi>
    <NavLi href="/icons" active={activeUrl === '/icons'}>Icons</NavLi>
    <NavLi href="https://github.com/shinokada/svelte-circle-flags">GitHub</NavLi>
    <NavLi href="https://svelte-svg-icons.vercel.app/">Icon sets</NavLi>
  </NavUl>
  <DarkMode />
</Navbar>
<div class="mx-16 mb-16">
  <slot />
</div>

<Footer footerType="logo" class="dark:bg-zinc-700 mx-8">
  <div class="sm:flex sm:items-center sm:justify-between">
    <FooterBrand
    href="https://svelte-circle-flags.vercel.app/"
    name="Svelte Circle Flags"
    classSpan="text-primary-700 dark:text-primary-500"
  />
  <FooterLinkGroup ulClass="flex flex-wrap items-center mt-3 text-sm text-gray-500 dark:text-gray-400 sm:mt-0">
    <FooterLink href="/">Home</FooterLink>
    <FooterLink href="/icons">Icons</FooterLink>
    <FooterLink href="https://github.com/shinokada/svelte-circle-flags/blob/main/LICENSE">Licensing</FooterLink>
    <FooterLink href="https://github.com/shinokada/svelte-circle-flags/">GitHub</FooterLink>
  </FooterLinkGroup>
  </div>
</Footer>


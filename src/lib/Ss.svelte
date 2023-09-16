<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of ss';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  width={size}
  height={size}
  class={$$props.class}
  {...$$restProps}
  {role}
  aria-label={ariaLabel}
  on:click
  on:keydown
  on:keyup
  on:focus
  on:blur
  on:mouseenter
  on:mouseleave
  on:mouseover
  on:mouseout
  viewBox="0 0 512 512"
  ><mask id="a"><circle cx="256" cy="256" r="256" fill="#fff" /></mask><g mask="url(#a)"
    ><path fill="#eee" d="M74.1 115 512 156.9v31.5l-42.4 70.3 42.4 64.2v31.5L74.1 386.8z" /><path
      fill="#333"
      d="M0 0h512v156.8H50z"
    /><path fill="#a2001d" d="M150.6 188.3H512v134.5H150.6z" /><path
      fill="#496e2d"
      d="M50 354.3h462V512H0z"
    /><path fill="#0052b4" d="M0 0v512l256-256z" /><path
      fill="#ffda44"
      d="m83.4 192.4 31.2 43.6 51.2-16.3-31.9 43.2 31.3 43.6-51-16.9-31.7 43.2.3-53.7L32 262.2 83 246z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of ss';
-->

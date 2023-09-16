<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of sc';
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
    ><path fill="#0052b4" d="M0 0v332l150.9-138.5L225.2 0z" /><path
      fill="#ffda44"
      d="M273.1 253.3 512 0H225.2L0 332v80.2z"
    /><path fill="#d80027" d="M512 0 0 412.2v50.4L277.9 390 512 256z" /><path
      fill="#eee"
      d="M0 462.6 512 256v133.5l-223.9 78.8L0 488.4z"
    /><path fill="#6da544" d="m512 389.5-512 99V512h512z" /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of sc';
-->

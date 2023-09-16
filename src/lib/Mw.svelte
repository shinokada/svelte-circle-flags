<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of mw';
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
    ><path fill="#d80027" d="m0 167 253.8-19.3L512 167v178l-254.9 32.3L0 345z" /><path
      fill="#333"
      d="M0 0h512v167H0z"
    /><path fill="#496e2d" d="M0 345h512v167H0z" /><path
      fill="#d80027"
      d="m332.5 122.4-31.2-14.7 16.6-30.3-34 6.5-4.3-34.3L256 75l-23.6-25.3L228 84l-34-6.5 16.7 30.3-31.3 14.7z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of mw';
-->

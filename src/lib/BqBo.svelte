<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of bq bo';
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
    ><path fill="#eee" d="M113.7 119.8 276 0h236v31.7L306 289.5 31.6 512H0V276z" /><path
      fill="#ffda44"
      d="M0 0v276L276 0H0z"
    /><path fill="#0052b4" d="M512 31.7 31.7 512H512V31.7z" /><path
      fill="#333"
      d="m255 245.7 22.1-12-22-12a78 78 0 0 0-65-65l-12-22-12 22a78 78 0 0 0-65 65l-22 12 22 12a78 78 0 0 0 65 65l12 22.1 12-22a78 78 0 0 0 65-65zm-77 32.6a44.5 44.5 0 1 1 0-89 44.5 44.5 0 0 1 0 89z"
    /><path
      fill="#d80027"
      d="m178 200.3 9.7 16.7H207l-9.6 16.7 9.6 16.7h-19.3l-9.6 16.7-9.7-16.7h-19.2l9.6-16.7-9.6-16.7h19.2z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of bq bo';
-->

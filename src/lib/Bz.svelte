<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of bz';
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
    ><path fill="#0052b4" d="m0 44.5 257.8-23.7L512 44.5v423l-252.5 26L0 467.5z" /><circle
      cx="256"
      cy="256"
      r="122.4"
      fill="#eee"
    /><circle cx="256" cy="256" r="100.2" fill="#6da544" /><circle
      cx="256"
      cy="256"
      r="66.8"
      fill="#eee"
    /><path fill="#0052b4" d="M256 239.3 219.8 256v27.8l36.2 22.3 36.2-22.3V256z" /><path
      fill="#ffda44"
      d="M219.8 222.6h72.4V256h-72.4z"
    /><path fill="#a2001d" d="M0 0h512v44.5H0zm0 467.5h512V512H0z" /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.codewithshin.com)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of bz';
-->

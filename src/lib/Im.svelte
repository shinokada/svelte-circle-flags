<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of im';
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
    ><path fill="#d80027" d="M0 0h512v512H0z" /><path
      fill="#eee"
      d="m350.8 171.6-18.1 64.6-54.3-10-35-72-94.4 33.4-7.4-21-24.7-3 18.6 52.5 65-16.7 18.4 52-44.9 66.3 76.3 65-14.5 17 9.7 22.9 36.1-42.3-46.8-48 35.8-42 79.8 5.8 18.2-98.6 22 4 15-19.8-54.8-10zM256 256z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of im';
-->

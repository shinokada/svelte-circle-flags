<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of au';
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
    ><path fill="#0052b4" d="M0 0h512v512H0z" /><path
      fill="#eee"
      d="m154 300 14 30 32-8-14 30 25 20-32 7 1 33-26-21-26 21 1-33-33-7 26-20-14-30 32 8zm222-27h47l-38 27 15-44 14 44zm7-162 7 15 16-4-7 15 12 10-15 3v17l-13-11-13 11v-17l-15-3 12-10-7-15 16 4zm57 67 7 15 16-4-7 15 12 10-15 3v16l-13-10-13 11v-17l-15-3 12-10-7-15 16 4zm-122 22 7 15 16-4-7 15 12 10-15 3v16l-13-10-13 11v-17l-15-3 12-10-7-15 16 4zm65 156 7 15 16-4-7 15 12 10-15 3v17l-13-11-13 11v-17l-15-3 12-10-7-15 16 4zM0 0v32l32 32L0 96v160h32l32-32 32 32h32v-83l83 83h45l-8-16 8-15v-14l-83-83h83V96l-32-32 32-32V0H96L64 32 32 0Z"
    /><path
      fill="#d80027"
      d="M32 0v32H0v64h32v160h64V96h160V32H96V0Zm96 128 128 128v-31l-97-97z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.codewithshin.com)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of au';
-->

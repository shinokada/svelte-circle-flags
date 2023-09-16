<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of nu';
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
    ><path fill="#ffda44" d="M0 256 256 0h256v512H0z" /><path
      fill="#eee"
      d="M0 0v32l32 32L0 96v160h32l32-32 32 32h32l42-16 41 16h45l-8-16 8-15v-14l-16-42 16-41V96l-32-32 32-32V0H96L64 32 32 0Z"
    /><path fill="#0052b4" d="M128 256v-83l83 83zm128-45-83-83h83z" /><path
      fill="#d80027"
      d="m128 128 128 128v-31l-97-97Z"
    /><path fill="#d80027" d="M32 0v32H0v64h32v160h64V96h160V32H96V0Z" /><circle
      cx="64"
      cy="64"
      r="48"
      fill="#0052b4"
    /><path
      fill="#ffda44"
      d="m50 198 14-44 15 44-38-27h47zM162 86l14-44 15 44-38-27h47ZM64 17l28 86-73-53h90l-73 53Z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of nu';
-->

<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of pn';
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
    ><path fill="#0052b4" d="M256 0h256v512H0V256Z" /><path
      fill="#acabb1"
      d="m401 156-34 11-33-11-11-28 11-28h67l-11 28Z"
    /><path fill="#338af3" d="M289 156v122c0 60 78 78 78 78s78-18 78-78V156H289z" /><path
      fill="#6da544"
      d="M296 307c20 37 71 49 71 49s52-12 71-49l-71-118-71 118z"
    /><path
      fill="#ffda44"
      d="m445 277-78-121-78 121v1a62 62 0 0 0 7 29l71-110 71 110a62 62 0 0 0 7-29z"
    /><path
      fill="#eee"
      d="M0 0v32l32 32L0 96v160h32l32-32 32 32h32v-83l83 83h45l-8-16 8-15v-14l-83-83h83V96l-32-32 32-32V0H96L64 32 32 0Z"
    /><path
      fill="#d80027"
      d="M32 0v32H0v64h32v160h64V96h160V32H96V0Zm96 128 128 128v-31l-97-97z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of pn';
-->

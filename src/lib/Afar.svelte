<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of afar';
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
    ><path fill="#eee" d="m0 160 256-32 256 32v192l-256 32L0 352Z" /><path
      fill="#0052b4"
      d="M0 0h512v160H0Z"
    /><path fill="#496e2d" d="M0 352h512v160H0Z" /><path
      fill="#d80027"
      d="M0 0v512l256-256L0 0z"
    /><path
      fill="#ff9811"
      d="m345 229-12 11 40 40-40 40 11 11 40-40 40 40 11-11-40-40 40-40-11-11-40 40z"
    /><path fill="#d80027" d="m384 181 21 62-54-38h66l-53 39z" /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of afar';
-->

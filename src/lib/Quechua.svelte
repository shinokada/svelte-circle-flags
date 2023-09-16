<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of quechua';
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
    ><path fill="#4a1f63" d="M0 512h512v-70l-256-32L0 442Z" /><path
      fill="#0052b4"
      d="M0 442h512v-70l-256-32L0 372Z"
    /><path fill="#d80027" d="M0 0h512v70l-256 32L0 70Z" /><path
      fill="#ffda44"
      d="M0 70h512v70l-256 32L0 140Z"
    /><path fill="#eee" d="M0 140h512v70l-32 46 32 46v70H0v-70l32-46-32-46Z" /><path
      fill="#496e2d"
      d="M0 210h512v92H0z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of quechua';
-->

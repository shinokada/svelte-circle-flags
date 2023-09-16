<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of torres_strait_islands';
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
    ><path fill="#0052b4" d="m0 128 256-32 256 32v256l-256 32L0 384Z" /><path
      fill="#333"
      d="m0 96 256-32 256 32v32H0Z"
    /><path fill="#6da544" d="M0 0h512v96H0Z" /><path
      fill="#333"
      d="m0 416 256 32 256-32v-32H0Z"
    /><path fill="#6da544" d="M0 512h512v-96H0Z" /><path
      fill="#eee"
      d="M245 144c-106 32-101 112-67 186l-40 38 73-27v-98c24-35 66-35 90 0v98l73 27-40-38c34-74 39-154-67-186l-11 46-11-46zm11 83-9 27h-28l23 17-9 28 23-17 23 17-9-28 24-17h-29l-9-27z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of torres_strait_islands';
-->

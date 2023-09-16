<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of fr cp';
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
    ><path fill="#0052b4" d="M0 0h512v512H0Z" /><path
      fill="#fff"
      d="m256 52 204 204-204 204L52 256Z"
    /><path fill="#ff9811" d="m232 463 12-299h24l12 299z" /><path
      fill="#6da544"
      d="M293 172c31-14 42-23 90-22-40-18-77-23-108 0 9-23 27-54 59-77-55 9-82 36-86 68-14-32-55-45-100-45 50 27 36 27 73 63-32-5-68 9-104 50 49-27 72-18 104-14a90 90 0 0 0-41 86c36-45 31-32 77-72 18 40 40 49 49 86 9-37 0-77-18-91 36 14 68 23 86 50-9-63-50-72-81-82z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of fr cp';
-->

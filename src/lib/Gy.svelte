<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of gy';
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
    ><path fill="#6da544" d="M77.7 0H512v512H77.8z" /><path
      fill="#eee"
      d="M425.4 254.7 31.4 512h46.4L512 256 77.7 0H31.4z"
    /><path fill="#ffda44" d="M256 256 31.4 512l436.8-256L31.4 0z" /><path
      fill="#333"
      d="M0 0v1.8l219.6 253.8L0 510v2h31.4l256-256L31.4 0z"
    /><path fill="#d80027" d="M0 0v512l256-256L0 0z" /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of gy';
-->

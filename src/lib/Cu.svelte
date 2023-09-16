<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of cu';
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
    ><path
      fill="#0052b4"
      d="M0 0h512v102.4L483.8 151l28.2 53.8v102.4l-30.5 50.7 30.5 51.7V512H0l39.8-257z"
    /><path fill="#ff9811" d="M0 44.5v423V256z" /><path
      fill="#eee"
      d="M27.2 102.4v102.4H512V102.4H27.2zm0 204.8v102.4H512V307.2H27.2z"
    /><path fill="#d80027" d="M0 0v512l256-256L0 0z" /><path
      fill="#eee"
      d="m103.6 189.2 16.6 51h53.6l-43.4 31.6 16.6 51-43.4-31.5-43.4 31.5 16.6-51-43.4-31.6H87z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of cu';
-->

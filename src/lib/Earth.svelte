<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of earth';
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
      d="M302.7 233.7a103.1 103.1 0 0 0 0 206 103.1 103.1 0 0 0 0-206zm0 20c46 0 83 37 83 83s-37 83-83 83-83-37-83-83 37-83 83-83z"
    /><path
      fill="#eee"
      d="M209.4 72.3a103.1 103.1 0 0 0 0 206 103.1 103.1 0 0 0 0-206zm0 20c46 0 83 37 83 83s-37 83-83 83-83-37-83-83 37-83 83-83z"
    /><path
      fill="#eee"
      d="M302.7 72.3a103.1 103.1 0 0 0 0 206 103.1 103.1 0 0 0 0-206zm0 20c46 0 83 37 83 83s-37 83-83 83-83-37-83-83 37-83 83-83z"
    /><path
      fill="#eee"
      d="M349.2 153a103.1 103.1 0 0 0 0 206 103.1 103.1 0 0 0 0-206zm0 20c46 0 83 37 83 83s-37 83-83 83-83-37-83-83 37-83 83-83z"
    /><path
      fill="#eee"
      d="M209.4 233.7a103.1 103.1 0 0 0 0 206 103.1 103.1 0 0 0 0-206zm0 20c46 0 83 37 83 83s-37 83-83 83-83-37-83-83 37-83 83-83z"
    /><path
      fill="#eee"
      d="M162.8 153a103.1 103.1 0 0 0 0 206 103.1 103.1 0 0 0 0-206zm0 20c46 0 83 37 83 83s-37 83-83 83-83-37-83-83 37-83 83-83z"
    /><path
      fill="#eee"
      d="M256 153.1a103.1 103.1 0 0 0 0 206 103.1 103.1 0 0 0 0-206zm0 20c46 0 83 37 83 83 0 45.9-37 83-83 83s-83-37.1-83-83c0-46 37-83 83-83z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of earth';
-->

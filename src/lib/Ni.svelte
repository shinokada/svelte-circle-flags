<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of ni';
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
      fill="#338af3"
      d="M0 0h512v144.7l-41.4 111.7L512 367.3V512H0V367.3l41.5-107.9L0 144.7z"
    /><path fill="#eee" d="M0 144.7h512v222.6H0z" /><path
      fill="#ffda44"
      d="M256 178a78 78 0 1 0 0 156 78 78 0 0 0 0-156zm0 122.5a44.5 44.5 0 1 1 0-89 44.5 44.5 0 0 1 0 89z"
    /><path fill="#0052b4" d="M294.6 267.1 256 256l-38.6 11.1-12.8 22.3h102.8z" /><path
      fill="#338af3"
      d="M256 200.3 230.3 245l25.7 11 25.7-11.1z"
    /><path fill="#6da544" d="M217.4 267.1h77.2L281.7 245h-51.4z" /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.codewithshin.com)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of ni';
-->

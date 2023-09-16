<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of jm';
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
      fill="#333"
      d="M23.3 488.6 0 465V47.1l23.4-23.7 464 464 24.6-22.6V47.1l-24.5-22.7z"
    /><path
      fill="#6da544"
      d="M23.3 23.3 47.1 0h417.7l23.8 23.4-464 464L47 512h418l22.6-24.5z"
    /><path
      fill="#ffda44"
      d="M0 0v47.1L208.8 256 0 464.9V512h47.1L256 303.2 464.9 512H512v-47L303.1 256 512 47.2V0h-47.2L256 208.9 47 0z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of jm';
-->

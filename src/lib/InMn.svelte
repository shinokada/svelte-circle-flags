<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of in mn';
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
    ><path fill="#d80027" d="M0 0h512v73L256 96 0 73Z" /><path
      fill="#eee"
      d="M0 73h512v73l-256 23L0 146Z"
    /><path fill="#333" d="M0 146h512v73l-256 23L0 219Z" /><path
      fill="#ffda44"
      d="M0 219h512v74l-256 22L0 293Z"
    /><path fill="#4a1f63" d="M0 293h512v73l-256 23L0 366Z" /><path
      fill="#338af3"
      d="M0 366h512v73l-256 23L0 439Z"
    /><path fill="#6da544" d="M0 439h512v73H0z" /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of in mn';
-->

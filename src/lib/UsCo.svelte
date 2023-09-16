<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of us co';
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
    ><path fill="#0052b4" d="M0 0h512v167l-64 89 64 89v167H0V345l64-89-64-89Z" /><path
      fill="#eee"
      d="M0 167h512v178H0z"
    /><path
      fill="#d80027"
      d="M344.3 299.8A128 128 0 0 1 201.8 382 128 128 0 0 1 96 256a128 128 0 0 1 105.8-126 128 128 0 0 1 142.5 82.2L224 256z"
    /><circle cx="224" cy="256" r="64" fill="#ffda44" /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of us co';
-->

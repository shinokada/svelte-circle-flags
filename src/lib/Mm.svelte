<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of mm';
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
    ><path fill="#6da544" d="m0 167 253.8-19.3L512 167v178l-254.9 32.3L0 345z" /><path
      fill="#ffda44"
      d="M0 0h512v167H0z"
    /><path fill="#d80027" d="M0 345h512v167H0z" /><path
      fill="#eee"
      d="M431.5 216.5h-134L256 89l-41.4 127.6h-134l108.3 78.8L147.5 423 256 345l108.5 78-41.4-127.6z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of mm';
-->

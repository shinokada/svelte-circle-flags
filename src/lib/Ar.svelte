<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of ar';
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
    ><path fill="#338af3" d="M0 0h512v144.7L488 256l24 111.3V512H0V367.3L26 256 0 144.7z" /><path
      fill="#eee"
      d="M0 144.7h512v222.6H0z"
    /><path
      fill="#ffda44"
      d="m332.4 256-31.2 14.7 16.7 30.3-34-6.5-4.2 34.3-23.7-25.2-23.6 25.2-4.3-34.3-34 6.5 16.6-30.3-31.2-14.7 31.3-14.7L194 211l34 6.5 4.3-34.3 23.6 25.2 23.6-25.2 4.4 34.3 34-6.5-16.7 30.3z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.codewithshin.com)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of ar';
-->

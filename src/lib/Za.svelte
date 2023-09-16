<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of za';
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
    ><path fill="#eee" d="m0 0 192 256L0 512h47l465-189v-34l-32-33 32-33v-34L47 0Z" /><path
      fill="#333"
      d="M0 142v228l140-114z"
    /><path fill="#ffda44" d="M192 256 0 95v47l114 114L0 370v47z" /><path
      fill="#6da544"
      d="M512 223H223L0 0v94l161 162L0 418v94l223-223h289z"
    /><path fill="#d80027" d="M512 0H47l189 189h276z" /><path
      fill="#0052b4"
      d="M512 512H47l189-189h276z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of za';
-->

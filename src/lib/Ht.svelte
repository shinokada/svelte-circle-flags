<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of ht';
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
    ><path fill="#a2001d" d="m0 256 254.8-41.8L512 256v256H0z" /><path
      fill="#0052b4"
      d="M0 0h512v256H0z"
    /><path fill="#eee" d="m345 322.8-89-11.1-89 11V189.3h178z" /><circle
      cx="256"
      cy="267.1"
      r="44.5"
      fill="#0052b4"
    /><circle cx="256" cy="267.1" r="22.3" fill="#a2001d" /><path
      fill="#6da544"
      d="M222.6 211.5h66.8L256 244.9z"
    /><path fill="#ffda44" d="M244.9 233.7H267v66.8h-22z" /><path
      fill="#6da544"
      d="M291.6 293.8h-71.2l-53.4 29h178z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.codewithshin.com)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of ht';
-->

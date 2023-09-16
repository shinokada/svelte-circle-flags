<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of hn';
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
      d="M0 0h512v144.7l-40.5 112.6 40.5 110V512H0V367.3l42.2-114L0 144.7z"
    /><path fill="#eee" d="M0 144.7h512v222.6H0z" /><path
      fill="#338af3"
      d="m157.5 167 8.3 25.5h26.9L171 208.2l8.2 25.5-21.7-15.7-21.7 15.7 8.3-25.5-21.7-15.7h26.9zm0 111.3 8.3 25.5h26.9L171 319.5l8.2 25.5-21.7-15.7-21.7 15.7 8.3-25.5-21.7-15.7h26.9zm197-111.3 8.2 25.5h26.9l-21.7 15.7 8.3 25.5-21.7-15.7-21.7 15.7 8.2-25.5-21.7-15.7h26.9zm0 111.3 8.2 25.5h26.9l-21.7 15.7 8.3 25.5-21.7-15.7-21.7 15.7 8.2-25.5-21.7-15.7h26.9zM256 222.6l8.3 25.5H291L269.4 264l8.3 25.5-21.7-15.8-21.7 15.8 8.3-25.5-21.7-15.8h26.8z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of hn';
-->

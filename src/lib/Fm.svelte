<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of fm';
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
    ><path fill="#338af3" d="M0 0h512v512H0z" /><path
      fill="#eee"
      d="m256 111.3 11 34h35.8l-29 21 11.1 34-28.9-21-29 21 11.1-34-29-21H245zM111.3 256l34-11v-35.8l21 29 34-11.1-21 28.9 21 29-34-11.1-21 29V267zM256 400.7l-11-34h-35.8l29-21-11.1-34 28.9 21 29-21-11.1 34 29 21H267zM400.7 256l-34 11v35.8l-21-29-34 11.1 21-28.9-21-29 34 11.1 21-29V245z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of fm';
-->

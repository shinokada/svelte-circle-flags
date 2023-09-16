<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of us nc';
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
    ><path fill="#0052b4" d="M0 0h232l64 256-64 256H0Z" /><path
      fill="#d80027"
      d="M232 0h280v256l-140 64-140-64Z"
    /><path fill="#eee" d="M232 256h280v256H232Z" /><path fill="#0052b4" d="M0 0h232v512H0z" /><path
      fill="#eee"
      d="m91 294 65-47H76l65 47-25-76z"
    /><path
      fill="#ffda44"
      d="M24 224h40v64H24zm144 0h40v64h-40zM64 92v16H24v32h40v-16h104v16h40v-32h-40V92H64zm0 328v-16H24v-32h40v16h104v-16h40v32h-40v16z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of us nc';
-->

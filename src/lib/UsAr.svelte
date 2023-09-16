<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of us ar';
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
    ><path fill="#d80027" d="M0 0h512v512H0z" /><path
      fill="#0052b4"
      d="M256 70 5 256l251 186 251-186Z"
    /><path
      fill="#eee"
      d="M256 130 85 256l171 126 171-126Zm-13.4-5.7 34.7-25h-42.7l34.7 25L256 83.7ZM46.5 277.4l27.2-33.1-41.4 11.1 40.1 15L49 234.6Zm419 0-27.2-33.1 41.4 11.1-40.1 15 23.4-35.8zm-145.7-104 27.2-33.1-41.4 11.1 40.1 15-23.4-35.8zm70.3 52 27.2-33.1-41.4 11.1 40.1 15-23.4-35.8zm-197.9-52L165 140.3l41.4 11.1-40.1 15 23.4-35.8zm-70.3 52-27.2-33.1 41.4 11.1-40.1 15 23.4-35.8zm-13 104 27.2-33.1-41.5 11.1 40.2 15-23.4-35.8zm70.3 52 27.2-33.1-41.4 11.1 40.1 15-23.4-35.8zm63.5 46.9 34.7-24.9h-42.7l34.7 24.9-13.3-40.6zm160.4-98.9-27.2-33.1 41.5 11.1-40.2 15 23.4-35.8zm-70.3 52-27.2-33.1 41.4 11.1-40.1 15 23.4-35.8z"
    /><path
      fill="#0052b4"
      d="m242.7 204.7 34.7-25h-42.7l34.7 25-13.3-40.7zm-39.2 103 34.7-25h-42.7l34.7 25-13.3-40.7zm78.2 0 34.7-25h-42.7l34.7 25-13.3-40.7zm-39.1-4.4 34.7 25h-42.7l34.7-25L256 344ZM160 223h192v32H160z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of us ar';
-->

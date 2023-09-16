<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of vc';
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
    ><path fill="#ffda44" d="M378.5 0H133.7l-22.3 256 22.3 256h244.8l22.3-256z" /><path
      fill="#338af3"
      d="M133.7 512V0H0v512z"
    /><path
      fill="#6da544"
      d="M512 0H378.5v512H512zM200.4 322.8 156 256l44.5-66.8 44.7 66.8zm111.4 0L267.1 256l44.6-66.8 44.5 66.8zm-55.7 89L211.6 345l44.5-66.7 44.5 66.7z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of vc';
-->

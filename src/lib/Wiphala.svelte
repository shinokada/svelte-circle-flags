<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of wiphala';
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
    ><path fill="#eee" d="M0 73V0h73l439 439v73h-73Z" /><path
      fill="#ffda44"
      d="M73 0v73h73v73h73v73h74v74h73v73h73v73h73v-73l-73-73-73-73v-1l-73-73-74-73-73-73H73z"
    /><path
      fill="#ff9811"
      d="M146 0v73h73v73h74v73h73v74h73v73h73v-73l-73-74L293 73 219 0h-73z"
    /><path fill="#d80027" d="M219 0v73h74v73h73v73h73v74h73v-74l-73-73-73-73-73-73h-74z" /><path
      fill="#4a1f63"
      d="M293 0v73h73v73h73v73h73v-73l-73-73-73-73h-73z"
    /><path fill="#0052b4" d="M366 0v73h73v73h73V73L439 0h-73z" /><path
      fill="#6da544"
      d="M439 0v73h73V0Zm0 512v-73h-74v-73h-73v-73h-73v-74h-73v-73H73V73H0v73l73 73 73 73v1l73 73 73 73 73 73z"
    /><path
      fill="#0052b4"
      d="M366 512v-73h-74v-73h-73v-73h-73v-74H73v-73H0v73l73 74 146 146 73 73z"
    /><path fill="#4a1f63" d="M292 512v-73h-73v-73h-73v-73H73v-74H0v74l73 73 73 73 73 73z" /><path
      fill="#d80027"
      d="M219 512v-73h-73v-73H73v-74H0v74l73 73 73 73z"
    /><path fill="#ff9811" d="M146 512v-73H73v-73H0v73l73 73z" /><path
      fill="#ffda44"
      d="M73 512v-73H0v73z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of wiphala';
-->

<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of sz';
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
      fill="#ffda44"
      d="m0 144.7 256-20.5 256 20.5V178l-37.4 79 37.4 77v33.3l-256 24.1L0 367.3V334l37.7-77.3L0 178z"
    /><path fill="#333" d="M0 0h512v144.7H0z" /><path fill="#0052b4" d="M0 367.3h512V512H0z" /><path
      fill="#a2001d"
      d="M0 178h512v156H0z"
    /><path fill="#ffda44" d="M89.2 244.9h334V267h-334zm44.6-44.6h244.8v22.3H133.8z" /><path
      fill="#eee"
      d="m256.2 189.2-18 65.2 18 68.4c66.8 0 124-66.8 124-66.8s-57.2-66.8-124-66.8z"
    /><path fill="#333" d="M256.2 322.8c-66.8 0-124-66.8-124-66.8s57.2-66.8 124-66.8" /><path
      fill="#eee"
      d="M211.7 233.7h22.2v44.6h-22.2z"
    /><path fill="#333" d="M278.5 233.7h22.2v44.6h-22.2z" /><g
      fill="#0052b4"
      transform="translate(.2)"
      ><circle cx="89" cy="256" r="22.3" /><circle cx="423" cy="256" r="22.3" /></g
    ></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.codewithshin.com)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of sz';
-->

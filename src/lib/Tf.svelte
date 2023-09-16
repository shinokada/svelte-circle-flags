<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let ariaLabel = 'flag of tf';
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
    ><path fill="#0052b4" d="M256 0h256v512H0V256Z" /><path fill="#eee" d="M0 0h256v256H0z" /><path
      fill="#0052b4"
      d="M0 0h75v224H0z"
    /><path fill="#d80027" d="M149 0h75v224h-75z" /><path
      fill="#eee"
      d="m323 158 13 21h36v71l-27-43-37 59h18l19-34 39 70 39-70 19 34h18l-37-59-27 43v-39h16l12-20h-28v-12h36l13-21zm43 88h-40v14h40zm76 0h-40v14h40z"
    /><path
      fill="#eee"
      d="m301 181 13 38-34-23h42l-34 23zm166 0 13 38-34-23h42l-34 23zM339 282l13 38-34-23h42l-34 23zm90 0 13 38-34-23h42l-34 23zm-45 34 13 38-34-23h42l-34 23z"
    /></g
  ></svg
>

<!--
@component
[Go to docs](https://svelte-circle-flags.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let ariaLabel = 'flag of tf';
-->

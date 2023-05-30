<script>
  export let size = '24';
  export let ariaLabel = 'flag of kanuri';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  width={size}
  height={size}
  class={$$props.class}
  {...$$restProps}
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
    ><path fill="#ffda44" d="m0 167 256-32 256 32v178l-256 32L0 345Z" /><path
      fill="#496e2d"
      d="M0 345h512v167H0Z"
    /><path fill="#0052b4" d="M0 0h512v167H0Z" /><path
      fill="#ffda44"
      d="m373 373 36 112-94-69h117l-95 69z"
    /></g
  ></svg
>
<!--
@component
[Go to Document](https://svelte-ant-design-icons.codewithshin.com/)
## Props
@prop size = '24';
@prop ariaLabel = 'icon file name';
## Event
- on:click
- on:keydown
- on:keyup
- on:focus
- on:blur
- on:mouseenter
- on:mouseleave
- on:mouseover
- on:mouseout
-->

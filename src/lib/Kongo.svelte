<script>
  export let size = '24';
  export let ariaLabel = 'flag of kongo';
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
    ><path fill="#eee" d="m0 160 256-32 256 32v192l-256 32L0 352Z" /><path
      fill="#d80027"
      d="M0 0h512v160H0Z"
    /><path fill="#ffda44" d="M0 352h512v160H0Z" /><path
      fill="#333"
      d="M144 423 256 79l112 344L75 211h362z"
    /><path fill="#eee" d="m175 381 81-250 81 250-213-154h264z" /></g
  ></svg
>
<!--
@component
[Go to Document](https://svelte-circle-flags.codewithshin.com/)
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

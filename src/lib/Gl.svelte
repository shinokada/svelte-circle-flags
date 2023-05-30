<script>
  export let size = '24';
  export let ariaLabel = 'flag of gl';
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
    ><path fill="#d80027" d="m0 256 259-45.3L512 256v256H0z" /><path
      fill="#eee"
      d="M0 0h512v256H0z"
    /><path fill="#eee" d="M55.7 256a122.4 122.4 0 1 0 244.8 0l-123-24z" /><path
      fill="#d80027"
      d="M55.7 256a122.4 122.4 0 1 1 244.8 0z"
    /></g
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

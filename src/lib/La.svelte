<script>
  export let size = '24';
  export let ariaLabel = 'flag of la';
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
    ><path
      fill="#d80027"
      d="M0 0h512v144.8l-45.8 113L512 367.4V512H0V367.4l46.3-111.1L0 144.8z"
    /><path fill="#0052b4" d="M0 144.8h512v222.6H0z" /><circle
      cx="256"
      cy="256.1"
      r="89"
      fill="#eee"
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

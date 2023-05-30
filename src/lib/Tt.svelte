<script>
  export let size = '24';
  export let ariaLabel = 'flag of tt';
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
    ><path fill="#d80027" d="M0 110.2 110.2 0H512v401.8L401.8 512H0z" /><path
      fill="#eee"
      d="M110.2 0H63L0 63v47.2L401.8 512H449l63-63v-47.2z"
    /><path fill="#333" d="M512 512v-63L63 0H0v63l449 449z" /></g
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

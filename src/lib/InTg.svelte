<script>
  export let size = '24';
  export let ariaLabel = 'flag of in tg';
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
    ><path fill="#eee" d="M0 0h512v128l-256 64L0 128Z" /><path
      fill="#338af3"
      d="M0 128h512v128l-256 64L0 256Z"
    /><path fill="#ff9811" d="M0 256h512v128l-256 64L0 384Z" /><path
      fill="#496e2d"
      d="M0 384h512v128H0z"
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

<script>
  export let size = '24';
  export let ariaLabel = 'flag of wf';
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
    ><path fill="#d80027" d="M256 0h256v512H0V256Z" /><path fill="#eee" d="M0 0h256v256H0Z" /><path
      fill="#0052b4"
      d="M0 0h75v224H0Z"
    /><path fill="#d80027" d="M149 0h75v224h-75z" /><path
      fill="#eee"
      d="m384 232-72-72h144zm-24 24-72-72v144zm24 24-72 72h144zm24-24 72-72v144z"
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

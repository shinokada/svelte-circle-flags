<script>
	export let size = '24';
	export let ariaLabel = 'flag of es variant';
</script>

<svg
	xmlns="http://www.w3.org/2000/svg"
	width={size}
	height={size}
	class={$$props.class}
	{...$$restProps}
	aria-label={ariaLabel}
	viewBox="0 0 512 512"
	style="border-radius:50%"
	><path fill="#d80027" d="M0 0h512v128l-39.8 130.3L512 384v128H0V384l37.8-124L0 128z" /><path
		fill="#ffda44"
		d="M0 128h512v256H0z"
	/></svg
>

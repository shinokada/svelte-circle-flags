<script>
	export let size = '24';
	export let ariaLabel = 'flag of co';
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
	><path fill="#d80027" d="m0 384 255.8-29.7L512 384v128H0z" /><path
		fill="#0052b4"
		d="m0 256 259.5-31L512 256v128H0z"
	/><path fill="#ffda44" d="M0 0h512v256H0z" /></svg
>

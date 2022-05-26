<script>
	export let size = '24';
	export let ariaLabel = 'flag of bo';
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
	><path fill="#ffda44" d="m0 167 252.9-29.3L512 167v178l-255.7 25.7L0 345z" /><path
		fill="#d80027"
		d="M0 0h512v167H0z"
	/><path fill="#6da544" d="M0 345h512v167H0z" /></svg
>

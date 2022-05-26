<script>
	export let size = '24';
	export let ariaLabel = 'flag of et ti';
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
	><path fill="#d80027" d="M0 0h512v512H0l64-256Z" /><path
		fill="#ffda44"
		d="M0 0v512l256-256Zm404 168v176L300 202l168 54-168 54Z"
	/></svg
>

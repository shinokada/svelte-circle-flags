<script>
	export let size = '24';
	export let ariaLabel = 'flag of sl';
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
	><path fill="#eee" d="m0 167 253.8-19.3L512 167v178l-254.9 32.3L0 345z" /><path
		fill="#6da544"
		d="M0 0h512v167H0z"
	/><path fill="#338af3" d="M0 345h512v167H0z" /></svg
>

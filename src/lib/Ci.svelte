<script>
	export let size = '24';
	export let ariaLabel = 'flag of ci';
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
	><path fill="#eee" d="M167 0h178l31 253.2L345 512H167l-33.4-257.4z" /><path
		fill="#ff9811"
		d="M0 0h167v512H0z"
	/><path fill="#6da544" d="M345 0h167v512H345z" /></svg
>

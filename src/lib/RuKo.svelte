<script>
	export let size = '24';
	export let ariaLabel = 'flag of ru ko';
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
	><path fill="#6da544" d="m0 167 256-32 256 32v178l-256 32L0 345Z" /><path
		fill="#eee"
		d="M0 345h512v167H0Z"
	/><path fill="#0052b4" d="M0 0h512v167H0Z" /></svg
>

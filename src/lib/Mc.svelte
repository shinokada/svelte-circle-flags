<script>
	export let size = '24';
	export let ariaLabel = 'flag of mc';
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
	><path fill="#eee" d="m0 256 258.2-43.3L512 256v256H0z" /><path
		fill="#d80027"
		d="M0 0h512v256H0z"
	/></svg
>

<script>
	export let size = '24';
	export let ariaLabel = 'flag of to';
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
	><path fill="#d80027" d="M0 256 256 0h256v512H0z" /><path fill="#eee" d="M0 0h256v256H0z" /><path
		fill="#d80027"
		d="M167 133.6v-33.4h-33.4v33.4h-33.4V167h33.4v33.3H167V167h33.3v-33.4z"
	/></svg
>

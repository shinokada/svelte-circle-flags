<script>
	export let size = '24';
	export let ariaLabel = 'flag of mt';
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
	><path fill="#eee" d="M0 0h256l52 259.2L256 512H0z" /><path
		fill="#d80027"
		d="M256 0h256v512H256z"
	/><path
		fill="#acabb1"
		d="M178 100.2V66.8h-33.3v33.4h-33.4v33.4h33.4V167h33.4v-33.4h33.4v-33.4z"
	/></svg
>

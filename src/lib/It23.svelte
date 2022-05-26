<script>
	export let size = '24';
	export let ariaLabel = 'flag of it 23';
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
	><path fill="#333" d="M0 0h256l64 256-64 256H0Z" /><path
		fill="#d80027"
		d="M256 0h256v512H256Z"
	/></svg
>

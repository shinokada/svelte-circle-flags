<script>
	export let size = '24';
	export let ariaLabel = 'flag of tt';
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
	><path fill="#d80027" d="M0 110.2 110.2 0H512v401.8L401.8 512H0z" /><path
		fill="#eee"
		d="M110.2 0H63L0 63v47.2L401.8 512H449l63-63v-47.2z"
	/><path fill="#333" d="M512 512v-63L63 0H0v63l449 449z" /></svg
>

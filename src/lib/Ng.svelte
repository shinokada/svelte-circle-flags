<script>
	export let size = '24';
	export let ariaLabel = 'flag of ng';
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
	><path fill="#6da544" d="M0 0h167l86 41.2L345 0h167v512H345l-87.9-41.4L167 512H0z" /><path
		fill="#eee"
		d="M167 0h178v512H167z"
	/></svg
>

<script>
	export let size = '24';
	export let ariaLabel = 'flag of ch';
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
	><path fill="#d80027" d="M0 0h512v512H0z" /><path
		fill="#eee"
		d="M389.6 211.5h-89v-89h-89.1v89h-89v89h89v89h89v-89h89z"
	/></svg
>

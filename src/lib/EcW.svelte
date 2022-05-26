<script>
	export let size = '24';
	export let ariaLabel = 'flag of ec w';
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
	><path fill="#eee" d="m0 167 254.6-36.6L512 166.9v178l-254.6 36.4L0 344.9z" /><path
		fill="#6da544"
		d="M0 0h512v166.9H0z"
	/><path fill="#0052b4" d="M0 344.9h512V512H0z" /></svg
>

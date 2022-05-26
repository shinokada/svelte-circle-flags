<script>
	export let size = '24';
	export let ariaLabel = 'flag of bq sa';
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
	><path fill="#d80027" d="M0 0h512v256H0z" /><path fill="#0052b4" d="M0 256h512v256H0z" /><path
		fill="#eee"
		d="M0 256 256 0l256 256-256 256z"
	/><path
		fill="#ffda44"
		d="m256 133.6 27.6 85H373L300.7 271l27.6 85-72.3-52.5-72.3 52.6 27.6-85-72.3-52.6h89.4z"
	/></svg
>

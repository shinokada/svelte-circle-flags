<script>
	export let size = '24';
	export let ariaLabel = 'flag of es cn';
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
	><path fill="#338af3" d="M167 0h178l32.3 257L345 512H167l-25.3-256z" /><path
		fill="#eee"
		d="M0 0h166.9v512H0z"
	/><path fill="#ffda44" d="M344.9 0H512v512H344.9z" /></svg
>

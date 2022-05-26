<script>
	export let size = '24';
	export let ariaLabel = 'flag of ru ta';
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
	><path fill="#eee" d="m0 224 256-32 256 32v64l-256 32L0 288Z" /><path
		fill="#496e2d"
		d="M0 0h512v224H0z"
	/><path fill="#d80027" d="M0 288h512v224H0z" /></svg
>

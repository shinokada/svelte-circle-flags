<script>
	export let size = '24';
	export let ariaLabel = 'flag of ru ba';
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
	><path fill="#eee" d="m0 160 256-32 256 32v192l-256 32L0 352Z" /><path
		fill="#338af3"
		d="M0 0h512v160H0Z"
	/><path fill="#496e2d" d="M0 352h512v160H0Z" /><circle
		cx="256"
		cy="256"
		r="64"
		fill="#ffda44"
	/></svg
>

<script>
	export let size = '24';
	export let ariaLabel = 'flag of kongo';
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
		fill="#d80027"
		d="M0 0h512v160H0Z"
	/><path fill="#ffda44" d="M0 352h512v160H0Z" /><path
		fill="#333"
		d="M144 423 256 79l112 344L75 211h362z"
	/><path fill="#eee" d="m175 381 81-250 81 250-213-154h264z" /></svg
>

<script>
	export let size = '24';
	export let ariaLabel = 'flag of cz';
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
	><path fill="#eee" d="M0 0h512v256l-265 45.2z" /><path
		fill="#d80027"
		d="M210 256h302v256H0z"
	/><path fill="#0052b4" d="M0 0v512l256-256L0 0z" /></svg
>

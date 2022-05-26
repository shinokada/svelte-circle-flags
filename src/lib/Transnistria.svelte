<script>
	export let size = '24';
	export let ariaLabel = 'flag of transnistria';
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
	><path fill="#a2001d" d="M0 0h512v189.5l-39 62 39 71.6V512H0V323l40.8-67L0 189.5z" /><path
		fill="#6da544"
		d="M0 189.5h512v133.6H0z"
	/></svg
>

<script>
	export let size = '24';
	export let ariaLabel = 'flag of gb sct';
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
	><path fill="#0052b4" d="M0 68 68 0h376l68 68v376l-68 68H68L0 444Z" /><path
		fill="#eee"
		d="M0 0v68l188 188L0 444v68h68l188-188 188 188h68v-68L324 256 512 68V0h-68L256 188 68 0H0z"
	/></svg
>

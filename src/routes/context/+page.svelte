<script>
  import { setContext } from 'svelte';
  import { Us, Jp } from '$lib';
  const iconCtx = {
    size: '100' // Icon size in pixels
  };
  setContext('iconCtx', iconCtx);
</script>

<Us />
<Jp />

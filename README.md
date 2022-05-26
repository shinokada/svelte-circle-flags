# Svelte-Circle-Flags

[![npm version](https://badgen.net/npm/v/svelte-circle-flags)](https://www.npmjs.com/package/svelte-circle-flags)
[![license](https://badgen.net/npm/license/svelte-circle-flags)](https://github.com/shinokada/svelte-circle-flags/blob/main/LICENSE)
[![downloads](https://badgen.net/npm/dm/svelte-circle-flags)](https://github.com/shinokada/svelte-circle-flags)

- [Circle-Flags](https://github.com/HatScripts/circle-flags)

## REPL

[Demo 1]()

## Icon Names

[Icon list](https://github.com/shinokada/svelte-circle-flags/blob/main/icon-list.md)

## ISO 3166 Country Codes

Most of the flags follow the ISO 3166 country codes.
[ISO 3166 Country Codes](https://github.com/shinokada/svelte-circle-flags/blob/main/iso-3166-country-codes.md)

## Installation

```sh
npm i -D svelte-circle-flags
```

## Size

Use the `size` prop to change the flag sizes.

```html
<script>
	import { Us, Ca, Fr, De, Dk, Jp, No, Ch, Cz } from 'svelte-circle-flags';
</script>

<div>
	<Us size="200" />
	<Ca size="200" />
	<Fr size="200" />
	<De size="200" />
	<Dk size="200" />
	<Jp size="200" />
	<No size="200" />
	<Ch size="200" />
	<Cz size="200" />
</div>
```

## CSS frameworks support

You can change size and other CSS using the `class` prop.

Tailwind CSS example:

```html
<Us class="rounded-full bg-white h-40 w-40 ring-2 ring-gray-300 m-4" />
```

Or you can use `size` and `class` props together.

```html
# Tailwind CSS
<Us class="rounded-full bg-white h-40 w-40 ring-2 ring-gray-300 m-4" />
# Tailwind CSS + Size
<Ca class="rounded-full bg-white ring-2 ring-gray-300 m-4" size="150" />
```

Bootstrap example:

```html
<Us class="position-absolute top-0 px-1" />
```

## aria-label

All icons have aria-label. For example `Us` has `aria-label="flag of us"`.
Use `ariaLabel` prop to modify the `aria-label` value.

```html
<Us ariaLabel="United States of America" />
```

## Passing down other attributes

You can pass other attibutes as well.

```html
<Us tabindex="0" />
```

## Using svelte:component

```html
<script>
	import { Ca } from 'svelte-circle-flags';
</script>

<svelte:component this="{Ca}" />
```

## Using onMount

```html
<script>
	import { ChatPlus } from 'svelte-circle-flags';
	import { onMount } from 'svelte';
	const props = {
		size: '50',
		color: '#ff0000'
	};
	onMount(() => {
		const icon = new Us({ target: document.body, props });
	});
</script>
```

## Import all

Use `import * as Icon from 'svelte-circle-flags`.

[REPL]()

```html
<script>
	import * as Icon from 'svelte-circle-flags';
</script>
<h1>Size</h1>
<Icon.Fr size="30" />
<Icon.De size="40" />

<h1>CSS HEX color</h1>
<Icon.Dk color="#c61515" size="40" />

<h1>Tailwind CSS</h1>
<Icon.Jp class="text-blue-500" />
<Icon.No class="text-pink-700" />
```

## Credit

All the credits goes to [Circle-Flags](https://github.com/HatScripts/circle-flags)

## Other icons

- [Svelte-Icon-Sets](https://svelte-svg-icons.vercel.app/)
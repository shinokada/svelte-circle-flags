<h1 align="center">Svelte Circle Flags</h1>
<p align="center">
<a href="https://svelte-circle-flags.codewithshin.com/">Svelte-Circle-Flags</a>
</p>

<p align="center">
<a href="https://github.com/sponsors/shinokada" target="_blank"><img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86" height="25"></a>
<a href="https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps" target="_blank"><img src="https://img.shields.io/badge/PWA-enabled-brightgreen" alt="PWA Shield" height="25">
</a>
<a href="https://www.npmjs.com/package/svelte-circle-flags" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/v/svelte-circle-flags" alt="npm" height="25"></a>
<a href="https://twitter.com/shinokada" rel="nofollow" target="_blank"><img src="https://img.shields.io/badge/created%20by-@shinokada-4BBAAB.svg" alt="Created by Shin Okada" height="25"></a>
<a href="https://opensource.org/licenses/MIT" rel="nofollow" target="_blank"><img src="https://img.shields.io/github/license/shinokada/svelte-circle-flags" alt="License" height="25"></a>
<a href="https://www.npmjs.com/package/svelte-circle-flags" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/dw/svelte-circle-flags.svg" alt="npm" height="25"></a>
</p>

330+ SVG icons from Circle-Flags

Thank you for considering my open-source package. If you use it in a commercial project, please support me by sponsoring me on GitHub: https://github.com/sponsors/shinokada. Your support helps me maintain and improve this package for the benefit of the community.

<p align="center">
<img src="/static/images/circle-flags-optimized-650-1050.png" width="650" />
</p>

## REPL

[REPL](https://svelte.dev/repl/382095078be04da7a5008b7f5e41d5c8)

## Installation

```sh
npm i -D svelte-circle-flags
```

## Icon names

[Icon list](/icon-list.md)

## Icon images

[Icon images](/icon-images.md)

## ISO 3166 Country Codes

Most of the flags follow the ISO 3166 country codes.
[ISO 3166 Country Codes](https://github.com/shinokada/svelte-circle-flags/blob/main/iso-3166-country-codes.md)


## Usage

```html
<script>
  import { Us } from 'svelte-circle-flags';
</script>

<Us />
```

## Faster compiling

If you need only a few icons from this library in your Svelte app, import them directly. This can optimize compilation speed and improve performance by reducing the amount of code processed during compilation.

```html
<script>
  import Us from 'svelte-circle-flags/Us.svelte';
</script>

<Us />
```

If you are a TypeScript user, **install version 5.0.0 or above**.

As of March 2023, the `typescript@beta` version is now available:

```sh
pnpm i -D typescript@beta
```

To avoid any complaints from the editor, add `node16` or `nodenext` to `moduleResolution` in your tsconfig.json file.

```json
{
  //...
  "compilerOptions": {
    // ...
    "moduleResolution": "nodenext"
  }
}
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

## Unfocusable icon

If you want to make an icon unfocusable, add `tabindex="-1"`.

```html
<Us tabindex="-1" />
```

## Event forwarding

The following events are forwarded:

```
on:click 
on:change 
on:keydown 
on:keyup 
on:focus 
on:blur 
on:mouseenter 
on:mouseleave 
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
  import { Us } from 'svelte-circle-flags';
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

## PWA: Fast & Offline

This website can be downloaded and installed on your device for offline access as a Progressive Web App.

To install a PWA, look for the "Add to Home Screen" option in the browser's menu or settings. On most mobile devices, this option can be found by visiting the website, then selecting the "Options" or "Menu" button in the browser, and looking for the "Add to Home Screen" option. On some desktop browsers, right-click on the page and select "Install".

# Svelte Circle Flags

<div class="flex gap-2 my-8">
<a href="https://github.com/sponsors/shinokada" target="_blank"><img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86" alt="sponsor" height="25" style="height: 25px !important;"></a>
<a href="https://www.npmjs.com/package/svelte-circle-flags" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/v/svelte-circle-flags" alt="npm" height="25" style="height: 25px !important;"></a>
<a href="https://twitter.com/shinokada" rel="nofollow" target="_blank"><img src="https://img.shields.io/badge/created%20by-@shinokada-4BBAAB.svg" alt="Created by Shin Okada" height="25" style="height: 25px !important;"></a>
<a href="https://opensource.org/licenses/MIT" rel="nofollow" target="_blank"><img src="https://img.shields.io/github/license/shinokada/svelte-circle-flags" alt="License" height="25" style="height: 25px !important;"></a>
<a href="https://www.npmjs.com/package/svelte-circle-flags" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/dw/svelte-circle-flags.svg" alt="npm" height="25" style="height: 25px !important;"></a>
</div>

360+ SVG icons from Circle-Flags

Thank you for considering my open-source package. If you use it in a commercial project, please support me by sponsoring me on GitHub: https://github.com/sponsors/shinokada. Your support helps me maintain and improve this package for the benefit of the community.


## Repo

[GitHub Repo](https://github.com/shinokada/svelte-circle-flags)

## Original source

[HatScripts/circle-flags](https://github.com/HatScripts/circle-flags)

## License

[Svelte-Circle-Flags License](https://github.com/shinokada/svelte-circle-flags/LICENSE)

[HatScripts/circle-flags License](https://github.com/HatScripts/circle-flags/blob/gh-pages/LICENSE.md)

## Installation

```sh
pnpm i -D svelte-circle-flags
```

## ISO 3166 Country Codes

Most of the flags follow the ISO 3166 country codes.
[ISO 3166 Country Codes](https://github.com/shinokada/svelte-circle-flags/blob/main/iso-3166-country-codes.md)

## Usage

```html
<script>
  import { Icon } from 'svelte-circle-flags';
</script>

<Icon name="us" />
```

## Props

- @prop name;
- @prop width = "512";
- @prop height = "512";
- @prop role = 'img';
- @prop ariaLabel='icon name'

## IDE support

If you are using an LSP-compatible editor, such as VSCode, Atom, Sublime Text, or Neovim, hovering over a component name will display a documentation link, props, and events.

## Size

Use the `size` prop to change the flag sizes.

```html
<Icon name="us" width="100" height="100" />
```

If you are using Tailwind CSS, you can add a custom size using Tailwind CSS by including the desired classes in the class prop. For example:

```html
<Icon name="us" class="shrink-0 h-20 w-20" />
```

## CSS frameworks support

You can apply CSS framework color and other attributes directly to the icon component or its parent tag using the `class` prop.

Tailwind CSS example:

```html
<Icon name="us" class="rounded-full bg-white h-40 w-40 ring-2 ring-gray-300 m-4" />
```

Bootstrap example:

```html
<Icon name="us" class="position-absolute top-0 px-1" />
```

## aria-label

All icons have aria-label. For example `us` has `aria-label="us"`.
Use `ariaLabel` prop to modify the `aria-label` value.

```html
<Icon name="us" ariaLabel="flag of United States of America" />
```

## Unfocusable icon

If you want to make an icon unfocusable, add `tabindex="-1"`.

```html
<Icon name="us" tabindex="-1" />
```

## Event forwarding

The following events are forwarded:

- on:click
- on:keydown
- on:keyup
- on:focus
- on:blur
- on:mouseenter
- on:mouseleave
- on:mouseover
- on:mouseout

## Passing down other attributes

You can pass other attibutes as well.

```html
<Icon name="us" tabindex="0" />
```

## Using svelte:component

```html
<svelte:component this="{Icon}" name="us" />
```

## Using onMount

```html
<script>
  import { Icon } from 'svelte-circle-flags';
  import { onMount } from 'svelte';
  const props = {
    name: 'us',
    size: '50',
  };
  onMount(() => {
    const icon = new Icon({ target: document.body, props });
  });
</script>
```

## Import all

Use `import {Icon, icons} from 'svelte-circle-flags`.

```html
<script>
  import {Icon, icons} from 'svelte-circle-flags';
</script>

{#each Object.keys(icons) as name}
<div class="flex gap-4 items-center text-lg">
  <Icon name={name} bind:width={size} bind:height={size} class="shrink-0"/>
  {name}
</div>
{/each}
```

## Other icons

[Svelte-Icon-Sets](https://svelte-svg-icons.vercel.app/)

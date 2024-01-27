# Svelte Circle Flags

<div class="flex gap-2 my-8">
<a href="https://github.com/sponsors/shinokada" target="_blank"><img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86" alt="sponsor"></a>
<a href="https://www.npmjs.com/package/svelte-circle-flags" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/v/svelte-circle-flags" alt="npm" ></a>
<a href="https://twitter.com/shinokada" rel="nofollow" target="_blank"><img src="https://img.shields.io/badge/created%20by-@shinokada-4BBAAB.svg" alt="Created by Shin Okada" ></a>
<a href="https://opensource.org/licenses/MIT" rel="nofollow" target="_blank"><img src="https://img.shields.io/github/license/shinokada/svelte-circle-flags" alt="License" ></a>
<a href="https://www.npmjs.com/package/svelte-circle-flags" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/dw/svelte-circle-flags.svg" alt="npm" ></a>
</div>

360+ SVG icons from Circle-Flags

Thank you for considering my open-source package. If you use it in a commercial project, please support me by sponsoring me [on GitHub](https://github.com/sponsors/shinokada). Your support helps me maintain and improve this package for the benefit of the community.

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

## Props

- size = ctx.size || '24';
- role = ctx.role || 'img';
- ariaLabel = 'file name';

## IDE support

If you are using an LSP-compatible editor, such as VSCode, Atom, Sublime Text, or Neovim, hovering over a component name will display a documentation link, props, and events.

## Size

Use the `size` prop to change the flag sizes.

```html
<script>
  import { Us, Ca, Fr } from 'svelte-circle-flags';
</script>

<div>
  <Us size="200" />
  <Ca size="200" />
  <Fr size="200" />
</div>
```

If you are using Tailwind CSS, you can add a custom size using Tailwind CSS by including the desired classes in the class prop. For example:

```html
<Us class="shrink-0 h-20 w-20" />
```

## Setting Global Icon using setContext

You can establish global icon preferences in your Svelte application using `setContext`. This allows you to configure icon-related properties once and share them across multiple components. Here's how you can do it:

```html
<script>
  import { setContext } from 'svelte';

  // Define your global icon settings
  const iconCtx = {
    size: '100' // Icon size in pixels
  };
  setContext('iconCtx', iconCtx);
</script>
```

The `size` and `role` properties are optional, allowing you to fine-tune the appearance and accessibility of your icons as needed.

If you set `size`, icons can be customized with different colors. For example:

```html
<script>
  import { setContext } from 'svelte';
  import { Us } from 'svelte-circle-flags';
  const iconCtx = {
    size: '50'
  };
  setContext('iconCtx', iconCtx);
</script>

<Us ariaLabel="flag of America" />
```

Remember that you can set only one or two of these properties, allowing you to tailor icon settings to your specific design and accessibility requirements.

Feel free to mix and match these properties as needed to create visually appealing and accessible icons in your Svelte application.

## Creating a Default Icon Setting

You can create a config file, `/src/lib/icon.config.json`.

The `Icon` component serves as a wrapper for svelte:component, allowing you to establish a global default setting or expand the capabilities of a component.

To create a default global icon setting, follow these steps:

### Configuration File

Start by creating a configuration file named `/src/lib/icon.config.json` with the following structure:

```json
{
  "config1": {
    "size": 40
  },
  "config2": {
    "size": 50
  }
}
```

In this JSON file, you can define different configurations (config1 and config2 in this case) for your icons, specifying attributes like size, variation, and color.

### Implementation

In your Svelte page file, make use of the configurations from the JSON file:

```html
<script lang="ts">
  type IconConfig = {
    config1: {
      size: number;
    };
    config2: {
      size: number;
    };
  };
  import config from '$lib/icon.config.json';
  import { Icon, Us, Jp } from 'svelte-circle-flags';

  const iconConfig: IconConfig = config;
  const config1 = iconConfig.config1;
  const config2 = iconConfig.config2;
</script>

<Icon {...config1} icon="{Us}" />
<Icon {...config2} icon="{Jp}" />
```

We import the configurations from the JSON file and assign them to config1 and config2. We then utilize the Icon component with the spread attributes `{...config1}` and `{...config2}` to apply the respective configurations to each icon.

### Custom Default Icon

If you wish to create a custom default icon, you can follow these steps:

Create a Svelte component named `src/lib/MyIcon.svelte`:

```html
<script lang="ts">
  import type { ComponentType } from 'svelte';
  const config = {
    size: 30
  };
  import { Icon } from 'svelte-circle-flags';
  export let icon: ComponentType;
</script>

<Icon {...config} {icon} />
```

This component, `MyIcon.svelte`, accepts an `icon` prop which you can use to pass in the specific icon component you want to display. The default configuration is also applied to the icon.

### Implementation in a Page

To use your custom default icon in a Svelte page, do the following:

```html
<script>
  import MyIcon from '$lib/MyIcon.svelte';
  import { Us } from 'svelte-circle-flags';
</script>

<MyIcon icon="{Us}" />
```

Here, we import the `MyIcon` component and the `Us` icon. By passing the `Us` icon to the `icon` prop of MyIcon, you apply the default configuration to the icon.

## CSS frameworks support

You can apply CSS framework color and other attributes directly to the icon component or its parent tag using the `class` prop.

Tailwind CSS example:

```html
<Us class="rounded-full bg-white h-40 w-40 ring-2 ring-gray-300 m-4" />
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

## Other icons

[Svelte-Icon-Sets](https://svelte-svg-icons.vercel.app/)

# bluebox

## Ultra lightweight CEP component library

Bluebox will be a Vue, Svelte and Web Component library that aims to have:

1. A single require statement and entrypoint (no need for lists of CSS stylesheets per use)
2. Simple and intuitive syntax (no need for complicated nesting of `divs` with long classnames per single component)
3. Visually indistinguishable results from the host application (no ultra modern UI components that stick out like a sore thumb, full rebuild of [Magic Mirror](https://github.com/Inventsable/CEP-Magic-Mirror))
4. All app themes and colors handled automatically

## Installation

```bash
# For future use
npm install @inventsable/bluebox
```

```js
// Import desired components per file
import {adobe-checkbox, adobe-btn, adobe-toolbar} from 'bluebox'
```

## Example usage (compared to Spectrum):

### [Spectrum checkbox](http://opensource.adobe.com/spectrum-css/2.13.0/docs/#checkbox):

```html
<label class="spectrum-Checkbox">
  <input type="checkbox" class="spectrum-Checkbox-input" id="checkbox-0" />
  <span class="spectrum-Checkbox-box">
    <svg
      class="spectrum-Icon spectrum-UIIcon-CheckmarkSmall spectrum-Checkbox-checkmark"
      focusable="false"
      aria-hidden="true"
    >
      <use xlink:href="#spectrum-css-icon-CheckmarkSmall" />
    </svg>
    <svg
      class="spectrum-Icon spectrum-UIIcon-DashSmall spectrum-Checkbox-partialCheckmark"
      focusable="false"
      aria-hidden="true"
    >
      <use xlink:href="#spectrum-css-icon-DashSmall" />
    </svg>
  </span>
  <span class="spectrum-Checkbox-label">Checkbox</span>
</label>
```

### Bluebox checkbox

```html
<!-- Vue -->
<adobe-checkbox label="Checkbox" :checked="someVariable" />

<!-- Svelte -->
<adobe-checkbox label="Checkbox" checked="{someVariable}" />
```

Only see and code what you need to see and code.

## To Do

- Documentation and API first, think about the absolute best and ideal usage before making decisions.
- Study UI component differences between Illustrator, After Effects, Photoshop, InDesign and Premiere Pro
- Pure SVG and font versions of all icons and UI elements
- Build each in both Vue and Svelte
- Finalize component API:
- - Checkbox
- - Input (text, number)
- - Dropdown menu
- - Button
- - Toolbar (button group)
- - Divider

- Recreate vanilla AI and AE panels using Bluebox alone

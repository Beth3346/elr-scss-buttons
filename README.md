# Buttons

[![npm version](http://img.shields.io/npm/v/elr-scss-buttons.svg)](https://www.npmjs.org/package/elr-scss-buttons)
[![CI](https://github.com/Beth3346/elr-scss-buttons/actions/workflows/node.js.yml/badge.svg)](https://github.com/Beth3346/elr-scss-buttons/actions/workflows/node.js.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![npm](https://img.shields.io/npm/dm/elr-scss-buttons.svg?style=flat)](https://npmjs.com/package/elr-scss-buttons)
[![Netlify Status](https://api.netlify.com/api/v1/badges/580bb90b-17bc-453e-94b4-bce48a1622bf/deploy-status)](https://app.netlify.com/sites/elr-scss-buttons/deploys)

some scss mixins for buttons

## Installation

Download node at [nodejs.org](http://nodejs.org) and install it, if you haven't already.

```sh
npm install elr-scss-buttons
```

or

```sh
yarn add elr-scss-buttons
```

## Implementation

### Scss

```scss
.button {
  margin: 8px;
  @include elr-button;
  @include elr-button-context;
  @include elr-button-branded;
}
```

```scss
.button-raised {
  @include elr-button-raised;
}
```

```scss
.button-gradient {
  @include elr-button-gradient;
}
```

```scss
.button-glass {
  @include elr-button-glass;
}
```

```scss
.button-invert {
  @include elr-button(
    $config: (
      background-color: $primary-color,
      hover-color: #76d219,
      border-radius: 0,
    )
  );
  margin: 8px;
}
```

```scss
.button-group {
  @include elr-button-group;
}
```

```scss
.button-icon {
  @include elr-icon-button;
  margin: 8px;
}
```

```scss
.button-icon-round {
  @include elr-icon-button(
    $config: (
      round: true,
    )
  );
  margin: 8px;
}
```

### HTML

```html
<button class="button">Button</button>
```

```html
<button class="button button-pill">Button</button>
```

```html
<button class="button-invert">Button</button>
```

```html
<button class="button button-ghost">Button</button>
```

```html
<button class="button button-ghost button-pill">Button</button>
```

```html
<button class="button button-raised">Button</button>
```

```html
<button class="button button-gradient">Button</button>
```

```html
<button class="button button-glass">Button</button>
```

SEE LICENSE IN LICENSE.md

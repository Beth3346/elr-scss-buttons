# elr-scss-buttons

[![Netlify Status](https://api.netlify.com/api/v1/badges/580bb90b-17bc-453e-94b4-bce48a1622bf/deploy-status)](https://app.netlify.com/sites/elr-scss-buttons/deploys)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![npm](https://img.shields.io/npm/dm/elr-scss-buttons.svg?style=flat)](https://npmjs.com/package/elr-scss-buttons)

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
.elr-button {
  @include elr-button;
}
```

```scss
.elr-button-invert {
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
.elr-button-pill {
  @include elr-button(
    $config: (
      pill: true,
    )
  );
  margin: 8px;
}
```

```scss
.elr-button-ghost {
  @include elr-button(
    $config: (
      border-color: $primary-color,
      background-color: transparent,
    )
  );
  margin: 8px;
}
```

```scss
.elr-button-group {
  @include elr-button-group;
}
```

```scss
.elr-button-icon {
  @include elr-icon-button;
  margin: 8px;
}
```

```scss
.elr-button-icon-round {
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
<button class="elr-button">Button</button>
```

```html
<button class="elr-button-pill">Button</button>
```

```html
<button class="elr-button-invert">Button</button>
```

```html
<button class="elr-button-ghost">Button</button>
```

```html
<button class="elr-button elr-button-raised">Button</button>
```

```html
<button class="elr-button elr-button-gradient">Button</button>
```

```html
<button class="elr-button elr-button-glass">Button</button>
```

SEE LICENSE IN LICENSE.md

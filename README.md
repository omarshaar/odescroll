# ODE Scroll

Modern and lightweight scroll animation library built with CSS3. ODE Scroll helps you create smooth reveal and entrance effects as elements enter the viewport, without heavy dependencies or complex setup.

## Features

- Lightweight and easy to integrate
- CSS3-based motion effects
- Works with plain HTML and JavaScript
- Supports global and per-element configuration
- Minimal setup for landing pages, portfolios, and marketing sites

## Live Demo

Explore the live demo here:

- https://odescroll.eano-shop.com/

## Installation

### CDN

Add the stylesheet in the `<head>` section:

```html
<link rel="stylesheet" href="https://unpkg.com/odescroll@1.0.3/styles.css" />
```

Add the script before the closing `</body>` tag and initialize the library:

```html
<script src="https://unpkg.com/odescroll@1.0.3/odescroll.js"></script>
<script>
  odescroll.init();
</script>
```

### Package managers

```bash
npm install --save odescroll
```

```bash
yarn add odescroll
```

### Import in JavaScript

```js
import { odescroll } from "odescroll";
import "odescroll/styles.css";
```

## Usage

### 1. Initialize the library

Call the initializer after the document is ready:

```js
odescroll.init();
```

You can also pass custom options:

```js
odescroll.init({
  option: value
});
```

### Options

| Option | Type | Default | Accepted Values | Description |
|--------|------|---------|-----------------|-------------|
| transition | number | 0.8s | 0-∞ | Animation duration |
| easing | string | ease-out | custom | Animation easing |
| once | boolean | true | true/false | Trigger animation only once |
| oneDirection | boolean | true | true/false | Restrict motion to one direction |
| threshold | number | 0.8 | 0 - 1 | Visibility threshold |

### 2. Add scroll animations to elements

```html
<div data-odescroll-container>
  <div data-odescroll="fade-down">
    <!-- content -->
  </div>
</div>
```

With custom per-element settings:

```html
<div data-odescroll-container>
  <div
    data-odescroll="fade-down"
    data-odescroll-transition="5"
    data-odescroll-easing="ease-in"
  >
    <!-- content -->
  </div>
</div>
```

### Custom attributes

You can configure individual elements using:

- `data-odescroll-transition`
- `data-odescroll-easing`

## Example

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>ODE Scroll Example</title>
    <link rel="stylesheet" href="https://unpkg.com/odescroll@1.0.3/styles.css" />
  </head>
  <body>
    <div data-odescroll-container>
      <section data-odescroll="fade-up">
        <h1>Hello ODE Scroll</h1>
      </section>
    </div>

    <script src="https://unpkg.com/odescroll@1.0.3/odescroll.js"></script>
    <script>
      odescroll.init();
    </script>
  </body>
</html>
```

## License

This project is open for use and modification under its license terms.

## Support

For questions, improvements, or contributions, feel free to open an issue or reach out through the project repository.


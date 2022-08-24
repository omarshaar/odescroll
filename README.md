# Awesome animate on scroll
ODE Scroll is a modern and awesome animate on scroll library using CSS3. see demos and get started now.
## ⚙ installation

### CDN
Add styles in `<head>`:

```html
  <link rel="stylesheet" href="https://unpkg.com/odescroll@1.0.3/styles.css" />
```

Add script right before closing `</body>` tag, and initialize ODEScroll:
```html
  <script src="https://unpkg.com/odescroll@1.0.3/odescroll.js"></script>
  <script>
    odescroll.init();
  </script>
```

### package managers

* `npm install --save odescroll`
or * `yarn add odescoll`



#### import files
```js
  import { odescroll } from "odescroll"
  import "odescroll/styles.css"
```

## Usage

### 1- Initialize 

Call initialize function after dom content loaded
```js
  odescroll.init()
```

with Options
```js
  odescroll.init({
    option: value
  })
```

### Options Table

| option           |     dataType    |  default                 | values           | Description                                               |
|------------------|-----------------|--------------------------|------------------|-----------------------------------------------------------|
| transition       | number          |   0.8s                   | 0-∞              |                                                           |
| easing           | string          |   ease-out               | custem           |                                                           |
| once             | boolean         |   true                   | true/false       |                                                           |
| oneDirection     | boolean         |   true                   | true/false       |                                                           |
| threshold        | number          |   0.8                    | 0 - 1            |                                                           |



### custem options for each Element as Attribute

* data-odescroll-transition
* data-odescroll-easing

### 2- Set animation 

```html
  <div data-odescroll-container>
      <div data-odescroll="fade-down"> 
          <!-- children -->
      </div>
  </div>
```

with option

```html
  <div data-odescroll-container>
      <div data-odescroll="fade-down" data-odescroll-transition="5" data-odescroll-easing="ease-in"> 
          <!-- children -->
      </div>
  </div>
```



## Demos
* https://scroll.o-de.org/demos

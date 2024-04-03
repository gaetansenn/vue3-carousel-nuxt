# Vue3 Carousel Nuxt Module

This module integrates the [Vue 3 Carousel](https://github.com/ismail9k/vue3-carousel) component with Nuxt 3.

## Installation

```bash
npx nuxi@latest module add vue3-carousel-nuxt
```

or with Yarn:

```bash
npx nuxi@latest module add vue3-carousel-nuxt
```

## Usage

In your `nuxt.config.ts` (or `nuxt.config.js`), add the module:

```javascript
export default {
  modules: [
    'vue3-carousel-nuxt'
  ]
}
```

With this configuration, you can now use the `Carousel`, `Slide`, `Pagination`, and `Navigation` components in your project. If you want to add a prefix to these component names, you can add a `carousel` configuration to your `nuxt.config.ts`:

```javascript
export default {
  modules: [
    'vue3-carousel-nuxt'
  ],
  carousel: {
    prefix: 'MyPrefix'
  }
}
```

This will allow you to use the components with a prefix, like so: `<MyPrefixCarousel />`, `<MyPrefixSlide />`, etc.

## Styling

The module automatically imports the default styles of Vue 3 Carousel. If you want to customize the styles, you can override them in your own style sheets:

```css
/* Override Carousel styles in your CSS or SCSS files */
.carousel__slide {
  /* Your custom styles here */
}
```

Remember, you don't need to import the `carousel.css` again in your stylesheets, as the module already imports it. Simply write your custom styles in your CSS files.

## Further References

For detailed information about the Vue 3 Carousel component, its usage, options and events, please refer to the [official Vue 3 Carousel documentation](https://ismail9k.github.io/vue3-carousel/).

To contribute, submit issues or pull requests, visit the [Vue 3 Carousel GitHub repository](https://github.com/ismail9k/vue3-carousel).

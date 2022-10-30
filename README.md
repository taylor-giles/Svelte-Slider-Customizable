# Svelte-Slider-Customizable
A fork of [svelte-slider](https://github.com/korywka/svelte-slider) which adds more customization options to the slider component. The additional customization options are used by setting specific CSS variables in the scope used by the Slider component.

```html
<Slider on:change={(event) => console.log(event.detail)} value={[0, 1]} />

<style>
    :root {
      --sliderPrimary: #FF9800;
      --sliderSecondary: rgba(0, 0, 0, 0.05);

      /* These are the added options */
      --sliderSelected: #FFFF00;
      --sliderThumb: #00BB45;
      --sliderThumbSize: 16px;
      --sliderHeight: 2px;
      --sliderRadius: 2px;
    }
</style>
```

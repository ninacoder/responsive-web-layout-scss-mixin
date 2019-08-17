# responsive-web-layout-scss-mixin
Create dynamic calculations of CSS property to provide a better responsive layout on not standard viewports.

There are different techniques to handle responsive typography and property (e.g. padding, margin) out there.
Most of theme are based on using exclusevely Media Queries, which could be really overwelming to manage.

This SCSS mixin is essentially based on Mikhail Sharanda approach. It calculates dynamically the property value based on the device's size and it defines a min and max values to prevent element getting too big or too small.

This SASS/SCSS mixin requires only three key values to work:
- the property
- min value
- max value

```
h2 {
  @include fluid-property('font-size', 18, 48);
}
```

### Responsive technique
SCSS mixin based on Mikhail Sharanda original code.

`Codepen` - [https://codepen.io/sharanda/pen/eoLBWv]

`Article` - [https://www.creativebloq.com/how-to/build-adaptive-layouts-without-media-queries]

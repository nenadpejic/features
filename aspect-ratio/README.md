# Aspect Ratio

## Setting heigh dynamically according to width

The child elements padding-top and padding-bottom is calculated based on the parent elements width.

Padding value is entered as a percentage value of desired aspect ratio. e.g. For 4:3 AR you would enter 75%.

In order to display content within the "height-ctrl" element, that content needs to be positioned absolute and the "height-ctrl" element to relative.

- Set "width-ctrl" to desired `width`;
- Set "height-ctrl" `paddint-top: 75%`;
- Set "content" to `position: absolute`;

```html
<div class="width-ctrl">
  <div class="height-ctrl">
    <div class="content">Aspect ratio 4:3</div>
  </div>
</div>
```

## Setting width dynamically according to height

If you want the width to be dynamically set according to height, you need to use the img tag.

- Set "container" to desired `height`.
- Set "placeholder" to `height: 100%`.
- Set "content" to `position: absolute`.

```html
<div class="container">
  <img class="placeholder" src="" />
  <div class="content"></div>
</div>
```

## Some common aspect ratios and how to calculate them:

- 1:1 => 100%
- 4:3 => 75%
- 16:9 => 56.25%
- 16:10 => 62.5%

Calculating percentage if AR is known:

```
4:3 => 3 / 4 = 0.75 * 100 % = 75%
```

Calculating height if width and AR is known:

```
h = 400px * 0.75 = 300px
```

Calculating width if height and AR is known:

```
w = 300px / 0.75 = 400px
```

Calculating AR if width and height is known:

```
AR = 300px / 400px = 0.75 * 100%
```

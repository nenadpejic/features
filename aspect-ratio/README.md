# Linked List

The child elements padding-top and padding-bottom is calculated based on the parent elements width.

Padding value is entered as a percentage value of desired aspect ratio. e.g. For 4:3 AR you would enter 75%.

In order to display content within the "height-ctrl" element, that content needs to be positioned absolute and the "height-ctrl" element to relative.

Some common aspect ratios:

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

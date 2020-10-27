# Footer positioning

In order to have the footer "stick" to the bottom of the page when the page content dosen't fill up the whole page, but also have the footer be pushed down with the content when it does, you need to put the page content and footer in a container.

- Set .container to `min-height: 100vh` and `padding-bottom: x`;
- Set footer to `height: x` and `position: absolute`;

> NOTE: Container padding-bottom and footer height values need to be the same so best use a variable e.g. `--footerHeight: 3rem;`

```css
.container {
  min-height: 100vh;
  position: relative;
  box-sizing: border-box;
  padding-bottom: 3rem; /* needs to match */
}
footer {
  height: 3rem; /* needs to match */
  position: absolute;
  bottom: 0;
  width: 100%;
}
```

```html
<div class="container">
  <div class="page-content"></div>
  <footer>Footer content</footer>
</div>
```

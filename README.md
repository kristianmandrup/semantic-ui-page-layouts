Semantic UI Page layout examples
--------------------------------

[![Greenkeeper badge](https://badges.greenkeeper.io/kristianmandrup/semantic-ui-page-layouts.svg)](https://greenkeeper.io/)

The goal of this project is to demonstrate examples for various typical page layouts using Semantic UI. We want to achieve the following:

-	1) Fixed Top bar menu with toggable left Sidebar
-	2) Sticky Top bar menu with toggable left Sidebar
-	1) and 2) with a toggable right Sidebar also

Menu toggler from: http://semantic-ui.com/modules/sticky.html

-	Fixed Menu toggler which fades out when clicked to show Sidebar

```html
<div class="ui black big launch right attached fixed button">
  <i class="content icon"></i>
  <span class="text">Menu</span>
</div>
```

CSS for cool launch button :)

```
.launch.button {
    display: block;
}

.fixed.launch.button {
  position: fixed;
  top: 2.5em;
  left: 0px;
  width: 55px;
  height: auto;
  white-space: nowrap;
  overflow: hidden;
  transition: 0.3s width ease, 0.5s transform ease;
}


.fixed.launch.button .text {
  position: absolute;
  white-space: nowrap;
  top: auto;
  left: 54px;
  opacity: 0;
  transition: 0.3s opacity 0.3s;
}

.fixed.launch.button:hover {
  width: 130px;
}
.fixed.launch.button:hover .text {
  opacity: 1;
}

/* Position Change */
pushable.left.overlay .fixed.launch.button {
  transform: translate3d(0, 0, 0);
}
pushable.overlay.left.pushed .fixed.launch.button {
  transform: translate3d(260px, 0, 0);
}

```

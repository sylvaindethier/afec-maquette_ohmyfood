# How to use

* SVG w/ `id="logo"` so it can be used in HTML files:

  ```html
    <svg>
      <use xlink:href="${href-to-svg-file.svg}#logo"></use>
    </svg>
  ```

* SVG w/ `class="logo"` so it can be styled in CSS files with the `.logo` selector

* SVG w/ `fill="var(--logo--fill, currentColor)"` so it can be styled in CSS files to fill or color the SVG, `currentColor` is the inherited CSS `color` property _by default_:

  ```css
    ${selector} {
      --logo--fill: <color>;
      /* or */
      color: <color>;
    }
  ```

* SVG w/ `width="100%"` and `height="100%"` so it can be scaled in CSS files:

  ```css
    ${selector} {
      width: <length>;
      height: <length>;
    }
  ```

# main.css

A repository for the development of the Project CSS file. It includes both the whole `main.css` file as well as component files used to generate `main.css`. This way you can either pull in the whole file, as we do in Project or you can pull in the individual files as needed.

## Features

The project contains the following files, which combine to create the different sections of `main.css.`

### _base.css

Several base styles are included. These styles:

- provide basic typography settings that improve text readability
- protect against unwanted `text-shadow` during text highlighting
- tweak the default alignment of some elements (e.g.: `img`, `video`,
  `fieldset`, `textarea`)

### _helpers.css

Along with the base styles, we also provide some commonly used helper classes.

#### `.hidden`

The `hidden` class can be added to any element that you want to hide visually
and from screen readers. It could be an element that will be populated and
displayed later, or an element you will hide with JavaScript.

#### `.sr-only`

The `sr-only` class can be added to any element that you want to hide
visually, while still have its content accessible to screen readers.

#### `.invisible`

The `invisible` class can be added to any element that you want to hide
visually and from screen readers, but without affecting the layout.

As opposed to the `hidden` class that effectively removes the element from the
layout, the `invisible` class will simply make the element invisible while
keeping it in the flow and not affecting the positioning of the surrounding
content.

#### `.clearfix`

The `clearfix` class can be added to any element to ensure that it always fully
contains its floated children.

Over the years there have been many variants of the clearfix hack, but currently, we use the [micro clearfix](http://nicolasgallagher.com/micro-clearfix-hack/).

### _mqs.css

We include placeholder media queries to help you build up your mobile styles for
wider viewports and high-resolution displays. It's recommended that you adapt
these media queries based on the content of your site rather than mirroring the
fixed dimensions of specific devices.

If you do not want to take the _mobile first_ approach, you can simply edit or
remove these placeholder media queries. One possibility would be to work from
wide viewports down, and use `max-width` media queries instead (e.g.:
`@media only screen and (max-width: 480px)`).

### _print.css

Lastly, we provide some useful print styles that will optimize the printing
process, as well as make the printed pages easier to read.

At printing time, these styles will:

- strip all background colors, change the font color to black, and remove the
  `text-shadow` ??? done in order to help save printer ink and speed up the
  printing process
- underline and expand links to include the URL ??? done in order to allow users
  to know where to refer to<br>
  (exceptions to this are: the links that are
  [fragment identifiers](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a#attr-href),
  or use the
  [`javascript:` pseudo protocol](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/void#JavaScript_URIs))
- expand abbreviations to include the full description ??? done in order to allow
  users to know what the abbreviations stands for
- provide instructions on how browsers should break the content into pages and
  on [orphans/widows](https://en.wikipedia.org/wiki/Widows_and_orphans), namely,
  we instruct
  [supporting browsers](https://en.wikipedia.org/wiki/Comparison_of_layout_engines_%28Cascading_Style_Sheets%29#Grammar_and_rules)
  that they should:

  - ensure the table header (`<thead>`) is [printed on each page spanned by the
    table](https://web.archive.org/web/20180815150934/http://css-discuss.incutio.com/wiki/Printing_Tables)
  - prevent block quotations, preformatted text, images and table rows from
    being split onto two different pages
  - ensure that headings never appear on a different page than the text they
    are associated with
  - ensure that
    [orphans and widows](https://en.wikipedia.org/wiki/Widows_and_orphans) do
    [not appear on printed pages](https://css-tricks.com/almanac/properties/o/orphans/)

The print styles are included along with the other `css` to [avoid the
additional HTTP request](http://www.phpied.com/delay-loading-your-print-css/).
Also, they should always be included last, so that the other styles can be
overwritten.


## Browser support

We use the following browserlist configuration:

```
 " browserslist": [
    "> 0.5%",
    "last 2 versions",
    "Firefox ESR",
    "not dead",
    "IE 11"
  ],
```

[That configuration translates to this full list of browsers.](https://browserl.ist/?q=%22%3E+0.5%25%22%2C%22last+2+versions%22%2C%22Firefox+ESR%22%2C%22not+dead%22%2C%22IE+11%22)
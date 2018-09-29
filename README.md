# ultimatesassfontmixin
Ultimate Sass mixin to create @font-face

Create a font face by providing font name, font weight and style & path to file

```sass
  +font('Brandon',300,'normal','2F3E50_2_0','/fonts/brandon/')

Rendered as CSS:

```css
@font-face {
  font-family: "Brandon";
  src: url("/fonts/brandon/2F3E50_2_0");
  font-weight: 300;
  font-style: "normal";
  src: url("/fonts/brandon/2F3E50_2_0.eot");
  src: url("/fonts/brandon/2F3E50_2_0.eot?#iefix") format("embedded-opentype"), url("/fonts/brandon/2F3E50_2_0.woff2") format("woff2"), url("/fonts/brandon/2F3E50_2_0.woff") format("woff"), url("/fonts/brandon/2F3E50_2_0.ttf") format("truetype"); }

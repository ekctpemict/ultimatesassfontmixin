# ultimatesassfontmixin
Ultimate Sass mixin to create @font-face

Create a font face by providing font name, font weight and style, path to file & file types

```sass
+font('Brandon__default',300,'normal','2F3E50_2_0','/fonts/brandon/') // use all of types: eot, woff, woff2, ttf
+font('Brandon',300,'italic','2F3E50_1_0','/fonts/brandon/', ["eot","ttf"]) // use only custom types
```
Rendered as CSS:

```css
@font-face {
  font-family: "Brandon__default";
  font-weight: 300;
  font-style: "normal";
  src: url("/fonts/brandon/2F3E50_2_0.eot");
  src: url('url("/fonts/brandon/2F3E50_2_0.eot?#iefix") format("embedded-opentype"), url("/fonts/brandon/2F3E50_2_0.woff") format("woff"), url("/fonts/brandon/2F3E50_2_0.woff2") format("woff2"), url("/fonts/brandon/2F3E50_2_0.ttf") format("truetype")'); }

@font-face {
  font-family: "Brandon";
  font-weight: 300;
  font-style: "italic";
  src: url("/fonts/brandon/2F3E50_1_0.eot");
  src: url('url("/fonts/brandon/2F3E50_1_0.eot?#iefix") format("embedded-opentype"), url("/fonts/brandon/2F3E50_1_0.ttf") format("truetype")'); }
```

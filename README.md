<h1 align='center'>CODE SNIPPETS</h1>

<p align='center'>Just a little file I made to keep track of some code snippets. I figured I'd share.</p>

<br>
<br>

<h2 align='center'>HTML</h2>

<br>
Blank Image Template

```html
https://dummyimage.com/200x200/000/fff
```

<br>
Font Awesome Link

```html
<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css"
  integrity="sha512-KfkfwYDsLkIlwQp6LFnl8zNdLGxu9YAA1QvwINks4PhcElQSvqcyVLLD9aMhXd13uQjoXtEKNosOWaZqXgel0g=="
  crossorigin="anonymous"
  referrerpolicy="no-referrer"
/>
```

<br>
<br>

<h2 align='center'>CSS</h2>

<h3 align='center'>Box Shadows</h3>

<br>
0dp

- Top app bar (resting elevation) option 1
- Text button
- Standard side sheet

<!-- prettier-ignore -->
```css
--box-shadow__none: none;
```

<br>
1dp

- Search bar (resting elevation)
- Card (resting elevation)
- Switch

<!-- prettier-ignore -->
```css
--box-shadow__1dp:
0 1px 1px 0 rgb(0 0 0 / 0.14),
0 2px 1px -1px rgb(0 0 0 / 0.12),
0 1px 3px 0 rgb(0 0 0 / 0.2);
```

<br>
2dp

- Contained button (resting elevation)

<!-- prettier-ignore -->
```css
--box-shadow__2dp:
0 2px 2px 0 rgb(0 0 0 / 0.14),
0 3px 1px -2px rgb(0 0 0 / 0.12),
0 1px 5px 0 rgb(0 0 0 / 0.2);
```

<br>
3dp

- Refresh indicator Search bar (scrolled state)

<!-- prettier-ignore -->
```css
--box-shadow__3dp:
0 3px 4px 0 rgb(0 0 0 / 0.14),
0 3px 3px -2px rgb(0 0 0 / 0.12),
0 1px 8px 0 rgb(0 0 0 / 0.2);
```

<br>
4dp

- Top app bar (scrolled state)
- Top app bar (resting elevation) option 2

<!-- prettier-ignore -->
```css
--box-shadow__4dp:
0 4px 5px 0 rgb(0 0 0 / 0.14),
0 1px 10px 0 rgb(0 0 0 / 0.12),
0 2px 4px -1px rgb(0 0 0 / 0.2);
```

<br>
6dp

- Floating Action Button (FAB - resting elevation)
- Snackbar

<!-- prettier-ignore -->
```css
--box-shadow__6dp:
0 6px 10px 0 rgb(0 0 0 / 0.14),
0 1px 18px 0 rgb(0 0 0 / 0.12),
0 3px 5px -1px rgb(0 0 0 / 0.2);
```

<br>
8dp

- Standard bottom sheet
- Standard side sheet
- Bottom navigation bar
- Bottom app bar
- Menus
- Sub menus
- Card (when picked up)
- Contained button (pressed state)

<!-- prettier-ignore -->
```css
--box-shadow__8dp:
0 8px 10px 1px rgb(0 0 0 / 0.14),
0 3px 14px 2px rgb(0 0 0 / 0.12),
0 5px 5px -3px rgb(0 0 0 / 0.2);
```

<br>
9dp

- None specified

<!-- prettier-ignore -->
```css
--box-shadow__9dp:
0 9px 12px 1px rgb(0 0 0 / 0.14),
0 3px 16px 2px rgb(0 0 0 / 0.12),
0 5px 6px -3px rgb(0 0 0 / 0.2);
```

<br>
12dp

- Floating Action Button (FAB - pressed)

<!-- prettier-ignore -->
```css
--box-shadow__12:
0 12px 17px 2px rgb(0 0 0 / 0.14),
0 5px 22px 4px rgb(0 0 0 / 0.12),
0 7px 8px -4px rgb(0 0 0 / 0.2);
```

<br>
16dp

- Modal bottom sheet
- Modal side sheet
- Navigation drawer

<!-- prettier-ignore -->
```css
--box-shadow__16:
0 16px 24px 2px rgb(0 0 0 / 0.14),
0 6px 30px 5px rgb(0 0 0 / 0.12),
0 8px 10px -5px rgb(0 0 0 / 0.2);
```

<br>
24dp

- Dialog

<!-- prettier-ignore -->
```css
--box-shadow__24dp:
0 24px 38px 3px rgb(0 0 0 / 0.14),
0 9px 46px 8px rgb(0 0 0 / 0.12),
0 11px 15px -7px rgb(0 0 0 / 0.2);
```

<br>

<h3 align='center'>Comments</h3>

```css
/*=========================================================|
|  #SECTION                                                |
|=========================================================*/

```css
/*-------------------------------------|
|  #SUBSECTION                         |
|-------------------------------------*/
```

```css
/*
| Comment
*/
```

<br>

<h3 align='center'>Reset</h3>

<!-- prettier-ignore -->
```css
/*
| Set up a decent box model on the root element
*/
html {
  box-sizing: border-box;
}

/*
| Make all elements from the DOM inherit from the parent box-sizing
| Since `*` has a specificity of 0, it does not override the `html` value
| making all elements inheriting from the root box-sizing value
*/
*, *::before, *::after {
  box-sizing: inherit;
}

blockquote, figcaption, fieldset, address, article, caption, details, section,
summary, canvas, figure, footer, header, hgroup, iframe, legend, object,
output, strong, aside, audio, embed, label, small, table, tbody, tfoot, thead,
video, abbr, body, cite, code, form, html, main, mark, menu, ruby, samp, span,
time, del, dfn, div, img, ins, kbd, nav, pre, sub, sup, var, em, dd, dl, dt,
h1, h2, h3, h4, h5, h6, li, ol, td, th, tr, ul, a, b, i, p, q, s {
  margin: 0;
  border: 0;
  padding: 0;
  text-rendering: optimizeLegibility;
  text-size-adjust: none;
  font: inherit;
  font-size: 100%;
  vertical-align: baseline;
  -webkit-font-smoothing: antialiased;
}

article, aside, details, figcaption, figure, footer, header, hgroup, main,
menu, nav, section { display: block; }

body { line-height: 1; }

ol, ul { list-style: none; }

blockquote, q { quotes: none; }

blockquote::before, blockquote::after, q::before, q::after {
  content: '';
  content: none;
}

table {
  border-collapse: collapse;
  border-spacing: 0;
}

input {
  border-radius: 0;
  -webkit-appearance: none;
}

a{
  text-decoration: none;
}
```

<br>

<h3 align='center'>Theme Colors</h3>

<details>
<summary>Dracula</summary>

<br>
Background

```css
--clr-background__100: 233 4% 45%;
--clr-background__200: 234 5% 39%;
--clr-background__300: 235 7% 33%;
--clr-background__400: 235 9% 26%;
--clr-background__500: 231 15% 18%; /* Default */
--clr-background__600: 231 15% 17%;
--clr-background__700: 230 15% 15%;
--clr-background__800: 229 15% 14%;
--clr-background__900: 228 16% 13%;
```

<br>
Foreground

```css
--clr-foreground__100: 228 6% 53%;
--clr-foreground__200: 229 7% 48%;
--clr-foreground__300: 231 9% 43%;
--clr-foreground__400: 231 11% 37%;
--clr-foreground__500: 232 14% 31%; /* Default */
--clr-foreground__600: 231 14% 28%;
--clr-foreground__700: 231 15% 26%;
--clr-foreground__800: 229 14% 23%;
--clr-foreground__900: 229 15% 21%;
```

<br>
Text

```css
--clr-text__100: 60 30% 96%; /* Default */
--clr-text__200: 60 8% 87%;
--clr-text__300: 60 5% 79%;
--clr-text__400: 60 3% 72%;
--clr-text__500: 60 2% 65%;
--clr-text__600: 60 2% 60%;
--clr-text__700: 60 2% 54%;
--clr-text__800: 60 1% 49%;
--clr-text__900: 60 1% 45%;
```

<br>
Comment

```css
--clr-comment__100: 224 27% 67%;
--clr-comment__200: 224 27% 64%;
--clr-comment__300: 225 27% 60%;
--clr-comment__400: 225 27% 56%;
--clr-comment__500: 225 27% 51%; /* Default */
--clr-comment__600: 225 25% 47%;
--clr-comment__700: 224 25% 42%;
--clr-comment__800: 225 25% 39%;
--clr-comment__900: 225 25% 35%;
```

<br>
Cyan

```css
--clr-cyan__100: 190 95% 84%;
--clr-cyan__200: 190 95% 83%;
--clr-cyan__300: 190 96% 81%;
--clr-cyan__400: 190 96% 79%;
--clr-cyan__500: 191 97% 77%; /* Default */
--clr-cyan__600: 190 68% 70%;
--clr-cyan__700: 190 51% 64%;
--clr-cyan__800: 191 40% 58%;
--clr-cyan__900: 191 32% 53%;
```

<br>
Green

```css
--clr-green__100: 136 92% 75%;
--clr-green__200: 136 93% 73%;
--clr-green__300: 135 93% 71%;
--clr-green__400: 135 94% 68%;
--clr-green__500: 135 94% 65%; /* Default */
--clr-green__600: 135 73% 59%;
--clr-green__700: 135 59% 53%;
--clr-green__800: 136 51% 48%;
--clr-green__900: 136 51% 44%;
```

<br>
Orange

```css
--clr-orange__100: 31 100% 80%;
--clr-orange__200: 31 100% 78%;
--clr-orange__300: 31 100% 76%;
--clr-orange__400: 31 100% 74%;
--clr-orange__500: 31 100% 71%; /* Default */
--clr-orange__600: 31 74% 65%;
--clr-orange__700: 31 58% 59%;
--clr-orange__800: 31 47% 54%;
--clr-orange__900: 30 41% 49%;
```

<br>
Pink

```css
--clr-pink__100: 325 100% 82%;
--clr-pink__200: 326 100% 80%;
--clr-pink__300: 325 100% 78%;
--clr-pink__400: 326 100% 76%;
--clr-pink__500: 326 100% 74%; /* Default */
--clr-pink__600: 326 73% 67%;
--clr-pink__700: 325 56% 61%;
--clr-pink__800: 326 44% 55%;
--clr-pink__900: 326 37% 51%;
```

<br>
Purple

```css
--clr-purple__100: 265 87% 85%;
--clr-purple__200: 264 88% 83%;
--clr-purple__300: 264 89% 82%;
--clr-purple__400: 265 90% 80%;
--clr-purple__500: 265 89% 78%; /* Default */
--clr-purple__600: 265 61% 71%;
--clr-purple__700: 265 45% 64%;
--clr-purple__800: 265 35% 58%;
--clr-purple__900: 265 28% 53%;
```

<br>
Red

```css
--clr-red__100: 0 100% 77%;
--clr-red__200: 0 100% 75%;
--clr-red__300: 0 100% 72%;
--clr-red__400: 0 100% 70%;
--clr-red__500: 0 100% 67%; /* Default */
--clr-red__600: 0 77% 61%;
--clr-red__700: 0 62% 55%;
--clr-red__800: 0 50% 50%;
--clr-red__900: 0 50% 46%;
```

<br>
Yellow

```css
--clr-yellow__100: 64 88% 84%;
--clr-yellow__200: 64 89% 82%;
--clr-yellow__300: 65 90% 80%;
--clr-yellow__400: 65 91% 78%;
--clr-yellow__500: 65 92% 76%; /* Default */
--clr-yellow__600: 65 64% 69%;
--clr-yellow__700: 65 48% 63%;
--clr-yellow__800: 64 38% 57%;
--clr-yellow__900: 64 31% 52%;
```

</details>

<details>
<summary>Material Design</summary>

<br>
Blue Grey

```css
--clr-blue-grey__50: 204 15% 94%;
--clr-blue-grey__100: 198 16% 84%;
--clr-blue-grey__200: 200 15% 73%;
--clr-blue-grey__300: 200 16% 62%;
--clr-blue-grey__400: 200 15% 54%;
--clr-blue-grey__500: 200 18% 46%;
--clr-blue-grey__600: 199 18% 40%;
--clr-blue-grey__700: 199 18% 33%;
--clr-blue-grey__800: 200 18% 26%;
--clr-blue-grey__900: 200 19% 18%;
```

<br>
Grey

```css
--clr-grey__50: 0 0% 98%;
--clr-grey__100: 0 0% 96%;
--clr-grey__200: 0 0% 93%;
--clr-grey__300: 0 0% 88%;
--clr-grey__400: 0 0% 74%;
--clr-grey__500: 0 0% 62%;
--clr-grey__600: 0 0% 46%;
--clr-grey__700: 0 0% 38%;
--clr-grey__800: 0 0% 26%;
--clr-grey__900: 0 0% 13%;
```

<br>
Brown

```css
--clr-brown__50: 20 16% 93%;
--clr-brown__100: 16 16% 81%;
--clr-brown__200: 15 15% 69%;
--clr-brown__300: 16 15% 56%;
--clr-brown__400: 16 18% 47%;
--clr-brown__500: 16 25% 38%;
--clr-brown__600: 15 25% 34%;
--clr-brown__700: 14 26% 29%;
--clr-brown__800: 11 26% 24%;
--clr-brown__900: 9 28% 19%;
```

<br>
Deep Orange

```css
--clr-deep-orange__50: 6 71% 95%;
--clr-deep-orange__100: 14 100% 87%;
--clr-deep-orange__200: 14 100% 78%;
--clr-deep-orange__300: 14 100% 70%;
--clr-deep-orange__400: 14 100% 63%;
--clr-deep-orange__500: 14 100% 57%;
--clr-deep-orange__600: 14 91% 54%;
--clr-deep-orange__700: 14 80% 50%;
--clr-deep-orange__800: 14 82% 46%;
--clr-deep-orange__900: 14 88% 40%;
--clr-deep-orange__100--accent: 14 100% 75%;
--clr-deep-orange__200--accent: 14 100% 63%;
--clr-deep-orange__400--accent: 14 100% 50%;
--clr-deep-orange__700--accent: 12 100% 43%;
```

<br>
Orange

```css
--clr-orange__50: 37 100% 94%;
--clr-orange__100: 36 100% 85%;
--clr-orange__200: 36 100% 75%;
--clr-orange__300: 36 100% 65%;
--clr-orange__400: 36 100% 57%;
--clr-orange__500: 36 100% 50%;
--clr-orange__600: 33 100% 49%;
--clr-orange__700: 30 100% 48%;
--clr-orange__800: 27 100% 47%;
--clr-orange__900: 21 100% 45%;
--clr-orange__100--accent: 38 100% 75%;
--clr-orange__200--accent: 34 100% 63%;
--clr-orange__400--accent: 34 100% 50%;
--clr-orange__700--accent: 26 100% 50%;
```

<br>
Amber

```css
--clr-amber__50: 46 100% 94%;
--clr-amber__100: 45 100% 85%;
--clr-amber__200: 45 100% 75%;
--clr-amber__300: 46 100% 65%;
--clr-amber__400: 45 100% 58%;
--clr-amber__500: 45 100% 51%;
--clr-amber__600: 42 100% 50%;
--clr-amber__700: 38 100% 50%;
--clr-amber__800: 34 100% 50%;
--clr-amber__900: 26 100% 50%;
--clr-amber__100--accent: 48 100% 75%;
--clr-amber__200--accent: 47 100% 63%;
--clr-amber__400--accent: 46 100% 50%;
--clr-amber__700--accent: 40 100% 50%;
```

<br>
Yellow

```css
--clr-yellow__50: 55 100% 95%;
--clr-yellow__100: 54 100% 88%;
--clr-yellow__200: 54 100% 81%;
--clr-yellow__300: 54 100% 73%;
--clr-yellow__400: 54 100% 67%;
--clr-yellow__500: 54 100% 62%;
--clr-yellow__600: 49 98% 60%;
--clr-yellow__700: 43 96% 58%;
--clr-yellow__800: 37 95% 56%;
--clr-yellow__900: 28 92% 53%;
--clr-yellow__100--accent: 60 100% 78%;
--clr-yellow__200--accent: 60 100% 50%;
--clr-yellow__400--accent: 55 100% 50%;
--clr-yellow__700--accent: 50 100% 50%;
```

<br>
Lime

```css
--clr-lime__50: 66 71% 95%;
--clr-lime__100: 65 69% 86%;
--clr-lime__200: 66 71% 77%;
--clr-lime__300: 66 70% 68%;
--clr-lime__400: 66 70% 61%;
--clr-lime__500: 66 70% 54%;
--clr-lime__600: 64 60% 50%;
--clr-lime__700: 62 61% 44%;
--clr-lime__800: 60 63% 38%;
--clr-lime__900: 54 70% 30%;
--clr-lime__100--accent: 65 100% 75%;
--clr-lime__200--accent: 65 100% 63%;
--clr-lime__400--accent: 73 100% 50%;
--clr-lime__700--accent: 75 100% 46%;
```

<br>
Light Green

```css
--clr-light-green__50: 88 52% 94%;
--clr-light-green__100: 88 51% 86%;
--clr-light-green__200: 88 50% 76%;
--clr-light-green__300: 88 50% 67%;
--clr-light-green__400: 88 50% 60%;
--clr-light-green__500: 88 50% 53%;
--clr-light-green__600: 89 46% 48%;
--clr-light-green__700: 92 48% 42%;
--clr-light-green__800: 95 49% 36%;
--clr-light-green__900: 103 56% 26%;
--clr-light-green__100--accent: 88 100% 78%;
--clr-light-green__200--accent: 88 100% 67%;
--clr-light-green__400--accent: 93 100% 51%;
--clr-light-green__700--accent: 97 81% 48%;
```

<br>
Green

```css
--clr-green__50: 125 39% 94%;
--clr-green__100: 122 38% 84%;
--clr-green__200: 122 37% 74%;
--clr-green__300: 123 38% 64%;
--clr-green__400: 123 38% 57%;
--clr-green__500: 122 39% 49%;
--clr-green__600: 123 41% 45%;
--clr-green__700: 123 43% 39%;
--clr-green__800: 123 46% 34%;
--clr-green__900: 124 55% 24%;
--clr-green__100--accent: 137 77% 85%;
--clr-green__200--accent: 151 82% 68%;
--clr-green__400--accent: 151 100% 45%;
--clr-green__700--accent: 145 100% 39%;
```

<br>
Teal

```css
--clr-teal__50: 177 41% 91%;
--clr-teal__100: 175 41% 79%;
--clr-teal__200: 174 42% 65%;
--clr-teal__300: 174 42% 51%;
--clr-teal__400: 174 63% 40%;
--clr-teal__500: 174 100% 29%;
--clr-teal__600: 174 100% 27%;
--clr-teal__700: 173 100% 24%;
--clr-teal__800: 173 100% 21%;
--clr-teal__900: 170 100% 15%;
--clr-teal__100--accent: 166 100% 83%;
--clr-teal__200--accent: 166 100% 70%;
--clr-teal__400--accent: 165 82% 51%;
--clr-teal__700--accent: 172 100% 37%;
```

<br>
Cyan

```css
--clr-cyan__50: 187 72% 93%;
--clr-cyan__100: 187 71% 82%;
--clr-cyan__200: 187 72% 71%;
--clr-cyan__300: 187 71% 59%;
--clr-cyan__400: 187 71% 50%;
--clr-cyan__500: 187 100% 42%;
--clr-cyan__600: 187 100% 38%;
--clr-cyan__700: 186 100% 33%;
--clr-cyan__800: 185 100% 28%;
--clr-cyan__900: 182 100% 20%;
--clr-cyan__100--accent: 180 100% 76%;
--clr-cyan__200--accent: 180 100% 55%;
--clr-cyan__400--accent: 186 100% 50%;
--clr-cyan__700--accent: 188 100% 42%;
```

<br>
Light Blue

```css
--clr-light-blue__50: 199 94% 94%;
--clr-light-blue__100: 199 92% 85%;
--clr-light-blue__200: 199 92% 74%;
--clr-light-blue__300: 199 91% 64%;
--clr-light-blue__400: 199 92% 56%;
--clr-light-blue__500: 199 98% 48%;
--clr-light-blue__600: 200 97% 45%;
--clr-light-blue__700: 201 98% 41%;
--clr-light-blue__800: 202 98% 37%;
--clr-light-blue__900: 206 99% 31%;
--clr-light-blue__100--accent: 198 100% 75%;
--clr-light-blue__200--accent: 199 100% 63%;
--clr-light-blue__400--accent: 199 100% 50%;
--clr-light-blue__700--accent: 203 100% 46%;
```

<br>
Blue

```css
--clr-blue__50: 205 87% 94%;
--clr-blue__100: 207 89% 86%;
--clr-blue__200: 207 90% 77%;
--clr-blue__300: 207 89% 68%;
--clr-blue__400: 207 90% 61%;
--clr-blue__500: 207 90% 54%;
--clr-blue__600: 208 79% 51%;
--clr-blue__700: 210 79% 46%;
--clr-blue__800: 212 80% 42%;
--clr-blue__900: 216 85% 34%;
--clr-blue__100--accent: 217 100% 75%;
--clr-blue__200--accent: 218 100% 63%;
--clr-blue__400--accent: 218 100% 58%;
--clr-blue__700--accent: 224 100% 58%;
```

<br>
Indigo

```css
--clr-indigo__50: 231 44% 94%;
--clr-indigo__100: 232 45% 84%;
--clr-indigo__200: 231 44% 74%;
--clr-indigo__300: 230 44% 64%;
--clr-indigo__400: 231 44% 56%;
--clr-indigo__500: 231 48% 48%;
--clr-indigo__600: 232 50% 45%;
--clr-indigo__700: 232 54% 41%;
--clr-indigo__800: 233 57% 37%;
--clr-indigo__900: 235 66% 30%;
--clr-indigo__100--accent: 231 100% 77%;
--clr-indigo__200--accent: 231 99% 66%;
--clr-indigo__400--accent: 231 99% 62%;
--clr-indigo__700--accent: 231 99% 59%;
```

<br>
Deep Purple

```css
--clr-deep-purple__50: 264 45% 94%;
--clr-deep-purple__100: 261 46% 84%;
--clr-deep-purple__200: 261 46% 74%;
--clr-deep-purple__300: 262 47% 63%;
--clr-deep-purple__400: 262 47% 55%;
--clr-deep-purple__500: 262 52% 47%;
--clr-deep-purple__600: 260 54% 45%;
--clr-deep-purple__700: 258 58% 42%;
--clr-deep-purple__800: 255 61% 39%;
--clr-deep-purple__900: 251 69% 34%;
--clr-deep-purple__100--accent: 262 100% 77%;
--clr-deep-purple__200--accent: 256 100% 65%;
--clr-deep-purple__400--accent: 259 100% 56%;
--clr-deep-purple__700--accent: 265 100% 46%;
```

<br>
Purple

```css
--clr-purple__50: 292 44% 93%;
--clr-purple__100: 291 46% 83%;
--clr-purple__200: 291 47% 71%;
--clr-purple__300: 291 47% 60%;
--clr-purple__400: 291 47% 51%;
--clr-purple__500: 291 64% 42%;
--clr-purple__600: 287 65% 40%;
--clr-purple__700: 282 68% 38%;
--clr-purple__800: 277 70% 35%;
--clr-purple__900: 267 75% 31%;
--clr-purple__100--accent: 291 95% 75%;
--clr-purple__200--accent: 291 96% 62%;
--clr-purple__400--accent: 291 100% 49%;
--clr-purple__700--accent: 280 100% 50%;
```

<br>
Pink

```css
--clr-pink__50: 340 80% 94%;
--clr-pink__100: 339 81% 85%;
--clr-pink__200: 340 82% 76%;
--clr-pink__300: 340 83% 66%;
--clr-pink__400: 340 82% 59%;
--clr-pink__500: 340 82% 52%;
--clr-pink__600: 338 78% 48%;
--clr-pink__700: 336 78% 43%;
--clr-pink__800: 334 79% 38%;
--clr-pink__900: 328 81% 29%;
--clr-pink__100--accent: 340 100% 75%;
--clr-pink__200--accent: 340 100% 63%;
--clr-pink__400--accent: 339 100% 48%;
--clr-pink__700--accent: 333 84% 42%;
```

<br>
Red

```css
--clr-red__50: 351 100% 96%;
--clr-red__100: 354 100% 90%;
--clr-red__200: 0 73% 77%;
--clr-red__300: 0 69% 67%;
--clr-red__400: 1 83% 63%;
--clr-red__500: 4 90% 58%;
--clr-red__600: 1 77% 55%;
--clr-red__700: 0 65% 51%;
--clr-red__800: 0 66% 47%;
--clr-red__900: 0 73% 41%;
--clr-red__100--accent: 5 100% 75%;
--clr-red__200--accent: 0 100% 66%;
--clr-red__400--accent: 348 100% 55%;
--clr-red__700--accent: 0 100% 42%;
```

</details>

<br>
<br>

<h2 align='center'>SCSS</h2>

<h3 align='center'>Color Maps</h3>

<details>
<summary>Material Design</summary>

```scss
$colors: (
  blue-grey: (
    50: hsl(204, 15%, 94%),
    100: hsl(198, 16%, 84%),
    200: hsl(200, 15%, 73%),
    300: hsl(200, 16%, 62%),
    400: hsl(200, 15%, 54%),
    500: hsl(200, 18%, 46%),
    600: hsl(199, 18%, 40%),
    700: hsl(199, 18%, 33%),
    800: hsl(200, 18%, 26%),
    900: hsl(200, 19%, 18%),
  ),
  grey: (
    50: hsl(0, 0%, 98%),
    100: hsl(0, 0%, 96%),
    200: hsl(0, 0%, 93%),
    300: hsl(0, 0%, 88%),
    400: hsl(0, 0%, 74%),
    500: hsl(0, 0%, 62%),
    600: hsl(0, 0%, 46%),
    700: hsl(0, 0%, 38%),
    800: hsl(0, 0%, 26%),
    900: hsl(0, 0%, 13%),
  ),
  brown: (
    50: hsl(20, 16%, 93%),
    100: hsl(16, 16%, 81%),
    200: hsl(15, 15%, 69%),
    300: hsl(16, 15%, 56%),
    400: hsl(16, 18%, 47%),
    500: hsl(16, 25%, 38%),
    600: hsl(15, 25%, 34%),
    700: hsl(14, 26%, 29%),
    800: hsl(11, 26%, 24%),
    900: hsl(9, 28%, 19%),
  ),
  deep-orange: (
    50: hsl(6, 71%, 95%),
    100: hsl(14, 100%, 87%),
    200: hsl(14, 100%, 78%),
    300: hsl(14, 100%, 70%),
    400: hsl(14, 100%, 63%),
    500: hsl(14, 100%, 57%),
    600: hsl(14, 91%, 54%),
    700: hsl(14, 80%, 50%),
    800: hsl(14, 82%, 46%),
    900: hsl(14, 88%, 40%),
    100-accent: hsl(14, 100%, 75%),
    200-accent: hsl(14, 100%, 63%),
    400-accent: hsl(14, 100%, 50%),
    700-accent: hsl(12, 100%, 43%),
  ),
  orange: (
    50: hsl(37, 100%, 94%),
    100: hsl(36, 100%, 85%),
    200: hsl(36, 100%, 75%),
    300: hsl(36, 100%, 65%),
    400: hsl(36, 100%, 57%),
    500: hsl(36, 100%, 50%),
    600: hsl(33, 100%, 49%),
    700: hsl(30, 100%, 48%),
    800: hsl(27, 100%, 47%),
    900: hsl(21, 100%, 45%),
    100-accent: hsl(38, 100%, 75%),
    200-accent: hsl(34, 100%, 63%),
    400-accent: hsl(34, 100%, 50%),
    700-accent: hsl(26, 100%, 50%),
  ),
  amber: (
    50: hsl(46, 100%, 94%),
    100: hsl(45, 100%, 85%),
    200: hsl(45, 100%, 75%),
    300: hsl(46, 100%, 65%),
    400: hsl(45, 100%, 58%),
    500: hsl(45, 100%, 51%),
    600: hsl(42, 100%, 50%),
    700: hsl(38, 100%, 50%),
    800: hsl(34, 100%, 50%),
    900: hsl(26, 100%, 50%),
    100-accent: hsl(48, 100%, 75%),
    200-accent: hsl(47, 100%, 63%),
    400-accent: hsl(46, 100%, 50%),
    700-accent: hsl(40, 100%, 50%),
  ),
  yellow: (
    50: hsl(55, 100%, 95%),
    100: hsl(54, 100%, 88%),
    200: hsl(54, 100%, 81%),
    300: hsl(54, 100%, 73%),
    400: hsl(54, 100%, 67%),
    500: hsl(54, 100%, 62%),
    600: hsl(49, 98%, 60%),
    700: hsl(43, 96%, 58%),
    800: hsl(37, 95%, 56%),
    900: hsl(28, 92%, 53%),
    100-accent: hsl(60, 100%, 78%),
    200-accent: hsl(60, 100%, 50%),
    400-accent: hsl(55, 100%, 50%),
    700-accent: hsl(50, 100%, 50%),
  ),
  lime: (
    50: hsl(66, 71%, 95%),
    100: hsl(65, 69%, 86%),
    200: hsl(66, 71%, 77%),
    300: hsl(66, 70%, 68%),
    400: hsl(66, 70%, 61%),
    500: hsl(66, 70%, 54%),
    600: hsl(64, 60%, 50%),
    700: hsl(62, 61%, 44%),
    800: hsl(60, 63%, 38%),
    900: hsl(54, 70%, 30%),
    100-accent: hsl(65, 100%, 75%),
    200-accent: hsl(65, 100%, 63%),
    400-accent: hsl(73, 100%, 50%),
    700-accent: hsl(75, 100%, 46%),
  ),
  light-green: (
    50: hsl(88, 52%, 94%),
    100: hsl(88, 51%, 86%),
    200: hsl(88, 50%, 76%),
    300: hsl(88, 50%, 67%),
    400: hsl(88, 50%, 60%),
    500: hsl(88, 50%, 53%),
    600: hsl(89, 46%, 48%),
    700: hsl(92, 48%, 42%),
    800: hsl(95, 49%, 36%),
    900: hsl(103, 56%, 26%),
    100-accent: hsl(88, 100%, 78%),
    200-accent: hsl(88, 100%, 67%),
    400-accent: hsl(93, 100%, 51%),
    700-accent: hsl(97, 81%, 48%),
  ),
  green: (
    50: hsl(125, 39%, 94%),
    100: hsl(122, 38%, 84%),
    200: hsl(122, 37%, 74%),
    300: hsl(123, 38%, 64%),
    400: hsl(123, 38%, 57%),
    500: hsl(122, 39%, 49%),
    600: hsl(123, 41%, 45%),
    700: hsl(123, 43%, 39%),
    800: hsl(123, 46%, 34%),
    900: hsl(124, 55%, 24%),
    100-accent: hsl(137, 77%, 85%),
    200-accent: hsl(151, 82%, 68%),
    400-accent: hsl(151, 100%, 45%),
    700-accent: hsl(145, 100%, 39%),
  ),
  teal: (
    50: hsl(177, 41%, 91%),
    100: hsl(175, 41%, 79%),
    200: hsl(174, 42%, 65%),
    300: hsl(174, 42%, 51%),
    400: hsl(174, 63%, 40%),
    500: hsl(174, 100%, 29%),
    600: hsl(174, 100%, 27%),
    700: hsl(173, 100%, 24%),
    800: hsl(173, 100%, 21%),
    900: hsl(170, 100%, 15%),
    100-accent: hsl(166, 100%, 83%),
    200-accent: hsl(166, 100%, 70%),
    400-accent: hsl(165, 82%, 51%),
    700-accent: hsl(172, 100%, 37%),
  )
  cyan:
  (
    50: hsl(187, 72%, 93%),
    100: hsl(187, 71%, 82%),
    200: hsl(187, 72%, 71%),
    300: hsl(187, 71%, 59%),
    400: hsl(187, 71%, 50%),
    500: hsl(187, 100%, 42%),
    600: hsl(187, 100%, 38%),
    700: hsl(186, 100%, 33%),
    800: hsl(185, 100%, 28%),
    900: hsl(182, 100%, 20%),
    100-accent: hsl(180, 100%, 76%),
    200-accent: hsl(180, 100%, 55%),
    400-accent: hsl(186, 100%, 50%),
    700-accent: hsl(188, 100%, 42%),
  )
  light-blue:
  (
    50: hsl(199, 94%, 94%),
    100: hsl(199, 92%, 85%),
    200: hsl(199, 92%, 74%),
    300: hsl(199, 91%, 64%),
    400: hsl(199, 92%, 56%),
    500: hsl(199, 98%, 48%),
    600: hsl(200, 97%, 45%),
    700: hsl(201, 98%, 41%),
    800: hsl(202, 98%, 37%),
    900: hsl(206, 99%, 31%),
    100-accent: hsl(198, 100%, 75%),
    200-accent: hsl(199, 100%, 63%),
    400-accent: hsl(199, 100%, 50%),
    700-accent: hsl(203, 100%, 46%),
  )
  blue:
  (
    50: hsl(205, 87%, 94%),
    100: hsl(207, 89%, 86%),
    200: hsl(207, 90%, 77%),
    300: hsl(207, 89%, 68%),
    400: hsl(207, 90%, 61%),
    500: hsl(207, 90%, 54%),
    600: hsl(208, 79%, 51%),
    700: hsl(210, 79%, 46%),
    800: hsl(212, 80%, 42%),
    900: hsl(216, 85%, 34%),
    100-accent: hsl(217, 100%, 75%),
    200-accent: hsl(218, 100%, 63%),
    400-accent: hsl(218, 100%, 58%),
    700-accent: hsl(224, 100%, 58%),
  )
  indigo:
  (
    50: hsl(231, 44%, 94%),
    100: hsl(232, 45%, 84%),
    200: hsl(231, 44%, 74%),
    300: hsl(230, 44%, 64%),
    400: hsl(231, 44%, 56%),
    500: hsl(231, 48%, 48%),
    600: hsl(232, 50%, 45%),
    700: hsl(232, 54%, 41%),
    800: hsl(233, 57%, 37%),
    900: hsl(235, 66%, 30%),
    100-accent: hsl(231, 100%, 77%),
    200-accent: hsl(231, 99%, 66%),
    400-accent: hsl(231, 99%, 62%),
    700-accent: hsl(231, 99%, 59%),
  )
  deep-purple:
  (
    50: hsl(264, 45%, 94%),
    100: hsl(261, 46%, 84%),
    200: hsl(261, 46%, 74%),
    300: hsl(262, 47%, 63%),
    400: hsl(262, 47%, 55%),
    500: hsl(262, 52%, 47%),
    600: hsl(260, 54%, 45%),
    700: hsl(258, 58%, 42%),
    800: hsl(255, 61%, 39%),
    900: hsl(251, 69%, 34%),
    100-accent: hsl(262, 100%, 77%),
    200-accent: hsl(256, 100%, 65%),
    400-accent: hsl(259, 100%, 56%),
    700-accent: hsl(265, 100%, 46%),
  )
  purple:
  (
    50: hsl(292, 44%, 93%),
    100: hsl(291, 46%, 83%),
    200: hsl(291, 47%, 71%),
    300: hsl(291, 47%, 60%),
    400: hsl(291, 47%, 51%),
    500: hsl(291, 64%, 42%),
    600: hsl(287, 65%, 40%),
    700: hsl(282, 68%, 38%),
    800: hsl(277, 70%, 35%),
    900: hsl(267, 75%, 31%),
    100-accent: hsl(291, 95%, 75%),
    200-accent: hsl(291, 96%, 62%),
    400-accent: hsl(291, 100%, 49%),
    700-accent: hsl(280, 100%, 50%),
  )
  pink:
  (
    50: hsl(340, 80%, 94%),
    100: hsl(339, 81%, 85%),
    200: hsl(340, 82%, 76%),
    300: hsl(340, 83%, 66%),
    400: hsl(340, 82%, 59%),
    500: hsl(340, 82%, 52%),
    600: hsl(338, 78%, 48%),
    700: hsl(336, 78%, 43%),
    800: hsl(334, 79%, 38%),
    900: hsl(328, 81%, 29%),
    100-accent: hsl(340, 100%, 75%),
    200-accent: hsl(340, 100%, 63%),
    400-accent: hsl(339, 100%, 48%),
    700-accent: hsl(333, 84%, 42%),
  )
  red:
  (
    50: hsl(351, 100%, 96%),
    100: hsl(354, 100%, 90%),
    200: hsl(0, 73%, 77%),
    300: hsl(0, 69%, 67%),
    400: hsl(1, 83%, 63%),
    500: hsl(4, 90%, 58%),
    600: hsl(1, 77%, 55%),
    700: hsl(0, 65%, 51%),
    800: hsl(0, 66%, 47%),
    900: hsl(0, 73%, 41%),
    100-accent: hsl(5, 100%, 75%),
    200-accent: hsl(0, 100%, 66%),
    400-accent: hsl(348, 100%, 55%),
    700-accent: hsl(0, 100%, 42%),
  ),
);
```

</details>

<br>

<h3 align='center'>Comments</h3>

<br>
Always end section brackets 2 columns after last letter

```scss
//==========================================================
// #SECTION
//==========================================================

//--------------------------------------
// #SUBSECTION
//--------------------------------------
```

```scss
//
// Comment
//
```

<br>

<H3 align='center'>Framework</H3>

<br>

[Use This Template](https://github.com/ij3ph/scss-base)

<br>
Terminal

1. `npm install`
2. `npm start`

<br>
Terminal (Focused): End Compiling

`CTRL` + `C`

<br>
Terminal (When Project Is Finished)

`npm build`

<br>

<h3 align='center'>Functions</h3>

<br>
Slightly Lighten a Color

```scss
@function tint($color, $percentage) {
  @return mix(white, $color, $percentage);
}
```

<br>
Slightly Darken a Color

```scss
@function shade($color, $percentage) {
  @return mix(black, $color, $percentage);
}
```

<br>

<h3 align='center'>Type Scale</h3>

```scss
$type-scale: (
  minor-second: (
    100: 0.823rem,
    200: 0.878rem,
    300: 0.937rem,
    400: 1rem,
    500: 1.067rem,
    600: 1.138rem,
    700: 1.215rem,
    800: 1.296rem,
    900: 1.383rem,
  ),
  major-second: (
    100: 0.702rem,
    200: 0.79rem,
    300: 0.889rem,
    400: 1rem,
    500: 1.125rem,
    600: 1.266rem,
    700: 1.424rem,
    800: 1.602rem,
    900: 1.802rem,
  ),
  minor-third: (
    100: 0.579rem,
    200: 0.694rem,
    300: 0.833rem,
    400: 1rem,
    500: 1.2rem,
    600: 1.44rem,
    700: 1.728rem,
    800: 2.074rem,
    900: 2.488rem,
  ),
  major-third: (
    100: 0.512rem,
    200: 0.64rem,
    300: 0.8rem,
    400: 1rem,
    500: 1.25rem,
    600: 1.563rem,
    700: 1.953rem,
    800: 2.441rem,
    900: 3.052rem,
  ),
  perfect-fourth: (
    100: 0.422rem,
    200: 0.563rem,
    300: 0.75rem,
    400: 1rem,
    500: 1.333rem,
    600: 1.777rem,
    700: 2.369rem,
    800: 3.157rem,
    900: 4.209rem,
  ),
  augmented-fourth: (
    100: 0.354rem,
    200: 0.5rem,
    300: 0.707rem,
    400: 1rem,
    500: 1.414rem,
    600: 1.999rem,
    700: 2.827rem,
    800: 3.998rem,
    900: 5.653rem,
  ),
  perfect-fifth: (
    100: 0.296rem,
    200: 0.444rem,
    300: 0.667rem,
    400: 1rem,
    500: 1.5rem,
    600: 2.25rem,
    700: 3.375rem,
    800: 5.063rem,
    900: 7.594rem,
  ),
  golden-ratio: (
    100: 0.236rem,
    200: 0.382rem,
    300: 0.618rem,
    400: 1rem,
    500: 1.618rem,
    600: 2.618rem,
    700: 4.236rem,
    800: 6.854rem,
    900: 11.089rem,
  ),
);
```

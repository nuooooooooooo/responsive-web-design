# responsive-web-design
Notes and projects for the [Responsive Web Design Bootcamp](https://scrimba.com/course/gresponsive/) by Kevin Powell

## 1. CSS Fundamentals
### 1.a Margins and Paddings
By default, headings and paragraphs have a `margin-top` and `margin-bottom` equal to their font-size, except for H1 where it's a little bit smaller. 
--> For consistency, it is best to **turn off** the `margin-top` on typography related elements. That way we can use padding on the parent (see "Tip to self" below) and keep it the same size on all sides. Do the same with `margin-bottom` on last child item.
- Refresher : by default, **margins collapse into each other**, which means that if the element above has a margin of 50px and the one on the bottom has a margin of 50px also, the space between them will be 50px not 100px. However!! In flexbox and grid, margins DO NOT collapse !

`+ Tip to self:` Instead of adding a padding to first and last child elements so they don't touch the borders of the box, it's best to add the padding directly to the parent element to prevent repeating oneself.

### 1.b Inline

**Inline** elements only accept margins and paddings on the left and right, to be precise, it does accept paddings on the top and bottom but it won't change the position of the element and will only overlap any surrounding items.
 
#### 1.b.1 Styling links.
- Refresher : Styling links is made possible by working on the following pseudo-classes:
  - `a:link`
  - `a:visited`
  - `a:focus`
  - `a:hover`
  - `a:active`
Always include a hover and focus state.

### Practice time:
- Always put styling regarding to paragraphs in the body to prevent from repeating css.

## 2. Starting to think responsively
## 3. Stepping up our style
## 4. CSS Flexbox
## 5. CSS Grid
## 6. Final project

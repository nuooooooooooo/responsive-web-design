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
**Inline blocks** works like an inline element, but margins and paddings can be set on it. Good for styling buttons.
 
#### 1.b.1 Styling links.
- Refresher : Styling links is made possible by working on the following pseudo-classes:
  - `a:link`
  - `a:visited`
  - `a:focus`
  - `a:hover`
  - `a:active`
Always include a hover and focus state.

### 1.c Buttons
In general, Kevin uses a ratio of 1:2.5.

### Practice time:
- Always put styling regarding to paragraphs in the body to prevent from repeating css.

### 1.d Specificity
From lowest specificity to highest, we have :
- Element selectors (could be equaled to 1pt),
- Class selectors(could be equaled to 10pt),
- ID selectors (could be equaled to 110pts).

*How to know when to use what*
General rules are put in **element selectors** (body, headings, paragraphs, etc.)
Everything else is put in **class selectors**.

### 1.f Compound selectors

They look like this:
```css
.section-one .btn { ... }
.section-two .btn { ... }
```

## 2. Starting to think responsively
## 3. Stepping up our style
## 4. CSS Flexbox
## 5. CSS Grid
## 6. Final project

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

*A better way to name CSS classes*
Create a generic class then give more specific classes if needed.
Ex: for a two buttons, first set a class of .btn, then set a more specific class such as .btn-secondary or .btn-accent on the button that needs to be slightly different in style.

### 1.f Compound selectors

They look like this:
```css
.section-one .btn { ... }
.section-two .btn { ... }
```

### 1.g Inheritance

For elements that already have some styling (such as links with color and text-decoration), it is possible to give them the color and style of the text around them if we use `inherit` on the property.


## 2. Starting to think responsively

//
## 3. Stepping up our style

- Line height's default is 1.4, in general it is best to set it somewhere between 1.6/1.7, but it can be set to a smaller size for larger font sizes.
- A nice trick to have text match a background color is to set it to white or black in rgba and add an alpha of about 0.6 to 0.75 and the text will match with the background no matter how.

### 3.a Background images
If text has to overlay an image, it is best to set it as a bg img.  
``background-size: contain`` makes sure we can see the entire image.  
``background-size: container`` makes sure the image fills the entire space of a div  
``background-positon: top left / top right / bottom right / center`` positions the image at a certain place in the div.  


## 4. CSS Flexbox
### 4.a Flex default value
By defaultm flex is set to stretch, which means the background stretches to the size of the container.
## 5. CSS Grid
## 6. Final project

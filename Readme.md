## 📌 **CSS Interview Questions for 5+ Years Experience**

### 🎯 **Core & Theory**

1. Difference between `display: none` vs `visibility: hidden` vs `opacity: 0`
2. What is CSS specificity hierarchy? 
//
Inline styles 
ID selector
Class selector
Element selector 
//

2. What is the CSS Box Model? Explain border-box vs content-box
3. Explain CSS Specificity & how the browser resolves conflicts
4. Explain Cascade, Inheritance, and Priority order
5. What are pseudo-classes vs pseudo-elements? Examples
6. What is the difference between `rem`, `em`, `vh`, `vw`, and `%`
7. What is the stacking context? Explain z-index issues and fixes
8. What is Reflow vs Repaint? How to reduce them?
9. What is BEM methodology? Why use it?
10. Explain CSS variables — advantages vs SASS variables

---

### 🔥 **Layout & Positioning**

11. Difference between relative, absolute, fixed, sticky positioning
12. Flexbox — common properties & layout examples:

* `justify-content`, `align-items`, `align-content`
* `flex: 1`, `flex-wrap`, `flex-shrink`, `flex-basis`

13. Grid layout — how is it different from Flexbox?
14. When do you choose Grid vs Flex vs Float?
15. Box-alignment in grid vs flex
16. Create a 3-column layout without using flex/grid (float or inline-block approach)

---

### 📱 **Responsive & UI Practices**

17. What are media queries? Give examples (mobile-first vs desktop-first)
18. How do you make images responsive? `object-fit` vs background-image
19. What is Mobile First CSS and why?
20. Explain container queries — use cases
21. What is responsive typography? e.g. `clamp()`

---

### ✨ **Visuals — Animation & Effects**

22. Difference between `transform` vs `translate` vs `transition`
23. CSS animation performance tips (GPU acceleration)
24. What is `will-change` and when to avoid using it?
25. How to create a smooth hover effect with CSS only?

---

### 🧠 **Advanced / Real-World CSS**

26. Explain Critical CSS & how to lazy-load CSS
27. What is a CSS preprocessor? SASS vs LESS
28. What are CSS Modules? Pros/cons in React
29. Styled-Components vs Tailwind vs traditional CSS — when to use what?
30. CSS Architecture patterns you use:

* BEM
* ITCSS
* Atomic CSS

31. How to avoid global CSS conflicts?
32. Explain `content-visibility` and performance benefits
33. Explain `@layer` in modern CSS
34. Difference between static, fluid, and adaptive layouts
35. Vendor prefixing — handled by PostCSS? Why needed earlier?

---

### 🧩 **Browser & Debugging**

36. CSS debugging techniques in Chrome DevTools
37. What is FOUC (Flash of Unstyled Content)?
38. What is CLS (Cumulative Layout Shift)? How CSS affects it?
39. How to handle cross-browser UI bugs?
40. Why fonts cause layout shifts? How to fix? (`font-display`)

---

### 👨‍💻 **React-Specific CSS Questions**

41. Explain how CSS Modules work in React
42. Styled-components vs Emotion — major differences
43. Tailwind + React — benefits and drawbacks
44. CSS-in-JS performance issues — how to avoid?
45. How do you style components dynamically in React?

---

### 🧠 **Scenario-Based CSS Questions**

| Scenario                        | Expected Concept          |
| ------------------------------- | ------------------------- |
| Center a div                    | Flexbox / Grid / position |
| Two divs side by side           | Flex/Grid/inline-block    |
| Sticky header & overflow scroll | `position: sticky`        |
| Text ellipsis clamp             | `-webkit-line-clamp`      |
| Equal height cards              | Flexbox/Grid              |
| Responsive navbar               | Flex + Media queries      |


01.01. What is the Box model in CSS? Which CSS properties are a part of it?
### A rectangle box is wrapped around every HTML element. The box model is used to determine the height and width of the rectangular box. The CSS Box consists of Width and height (or in the absence of that, default values and the content inside), padding, borders, margin.

## 2- What are the different types of Selectors in CSS?
    - Universal Selector
    - Element Type Selector
    - ID Selector
    - Class Selector
    - Descendant Combinator
    - Child Combinator
    - General Sibling Combinator
    - Adjacent Sibling Combinator
    - Attribute Selector
## 3- What is VH/VW (viewport height/ viewport width) in CSS?

### It’s a CSS unit used to measure the height and width in percentage with respect to the viewport. It is used mainly in responsive design techniques. The measure VH is equal to 1/100 of the height of the viewport. If the height of the browser is 1000px, 1vh is equal to 10px. Similarly, if the width is 1000px, then 1 vw is equal to 10px.

## 4- Difference between reset vs normalize CSS?. How do they differ?

###  Reset CSS: CSS resets aim to remove all built-in browser styling. For example margins, paddings, font-sizes of all elements are reset to be the same. 
### Normalize CSS: Normalize CSS aims to make built-in browser styling consistent across browsers. It also corrects bugs for common browser dependencies.

## 5- What is the difference between inline, inline-block, and block Elements?

### Block Element: The block elements always start on a new line. They will also take space for an entire row or width. List of block elements are <div>, <p>.

### Inline Elements: Inline elements don't start on a new line, they appear on the same line as the content and tags beside them. Some examples of inline elements are <a>, <span> , <strong>, and <img> tags. 

### Inline Block Elements: Inline-block elements are similar to inline elements, except they can have padding and margins and set height and width values.

## 6- What are Pseudo elements and Pseudo classes?

### Pseudo-elements allows us to create items that do not normally exist in the document tree, for example ::after 
    ::before
    ::after
    ::first-letter
    ::first-line
    ::selection

### Pseudo-classes select regular elements but under certain conditions like when the user is hovering over the link.
    :link
    :visited
    :hover
    :active
    :focus

## 7- Does margin-top or margin-bottom have an effect on inline elements?

### No, it doesn’t affect the inline elements. Inline elements flow with the contents of the page.

## 8- What is cascading in CSS?

### “Cascading” refers to the process of going through the style declarations and defining weight or importance to the styling rules that help the browser to select what rules have to be applied in times of conflict. The conflict here refers to multiple rules that are applicable to a particular HTML element. In such cases, we need to let the browser know what style needs to be applied to the element. This is done by cascading down the list of style declarations elements.

For example, if we have the below style:

p{
    color:white;
}
and we also have the following declaration below it or in another stylesheet that has been linked to the page:

p{
    color: black;
}
We have a conflict in color property here for the paragraph elements. Here, the browser just cascades down to identify what is the most recent and most specific style and applies that. Since we have the color:black; as the most specific declaration, the color black is applied to the paragraph elements. Now if you want to ensure color white is applied to the paragraph, we can define weight to that style by adding !important as shown below:

p{
    color:white !important;
}
!important ensures that the property has the maximum weight in presence of other conflicting properties.

## What are the differences between adaptive design and responsive design?

### Adaptive Design	Responsive Design
Adaptive design focuses on developing websites based on multiple fixed layout sizes.	Responsive design focuses on showing content on the basis of available browser space.
When a website developed using adaptive design is opened on the desktop browser, first the available space is detected and then the layout with most appropriate sizes are picked and used for the display of contents. Resizing of browser window has no affect on the design.	When a website developed using responsive design is opened on a desktop browser and when we try to resize the browser window, the content of the website is dynamically and optimally rearranged to accomodate the window.
Usually, adaptive designs use six standard screen widths - 320 px, 480 px, 760 px, 960 px, 1200 px, 1600 px. These sizes are detected and appropriate layouts are loaded.	This design makes use of CSS media queries for changing styles depending on the target devices properties for adapting to different screens.
It takes a lot of time and effort to first examine the options and realities of the end users and then design best possible adaptive solutions them.	Generally, Responsive design takes much less work to build and design fluid websites that can accomodate content from screen depending on the screen size.
Gives a lot of control over the design to develop sites for specific screens.	No much control over the design is offered here.


## Differentiate between CSS3 and CSS2.

### The main difference between CSS3 and CSS2 is that CSS divides different sections into modules and supports many browsers. It also contains new General Sibling Combinators responsible for matching similar elements.

## Define z-index.
### This is one of the most frequently asked CSS interview questions. Z-index is used to specify the stack order of elements that overlap each other. Its default value is zero and can take both negative and positive values. A higher z-index value is stacked above the lower index element. It takes the following values- auto, number, initial, and inherit. 

## How can you use CSS to control image repetition?
###  background-repeat: none;

## Tell us about the property used for image scroll controlling?
###  background-attachment: fixed;



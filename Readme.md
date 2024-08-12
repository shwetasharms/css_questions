https://www.interviewbit.com/css-interview-questions/


## 1- What is the Box model in CSS? Which CSS properties are a part of it?
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



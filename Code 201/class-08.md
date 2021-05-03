
# Readings : CSS Layout
## Chapter15 :: "layout" 
* **Block-level elements** start on a new line.
* **Inline elements** flow in between surrounding text.

* **Controlling the Position of Elements**

![css-positioning](https://www.webideasole.com/wp-content/uploads/2019/02/css_positions-1024x349.png)

* CSS has the following positioning schemes that allow you to control the layout of a page:
     1. **Normal flow** <span style="color:red"> (position:static) </span> Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. Even if you specify the width of the boxes and there is space for two elements to sit  ide-byside, they will not appear next to each other. This is the default behavior (unless you tell the browser to do something else).
     2. **Relative Positioning** <span style="color:red"> (position:relative) </span> This moves an element from the position it would be in normal flow, shifting it to the  op, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding  elements; they stay in the position they would be in in normal flow.
     3. **Absolute positioning** <span style="color:red"> (position:absolute/fixed) </span> This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page.

![css-position-all](https://www.csssolid.com/images/csspositions/css-position-all.png)

* To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how  far from the top or bottom and left or right it should be placed.
     1. **Fixed Positioning** This is a form of absolute positioning that positions the element in relation to the browser window.
     2. **Floating Elements** Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow.
         * Using Float to Place El ements Side-by-Side.
         * The **clear property** allows you to say that no element (within the same containing element) should touch the sides of a box. It can take the following values:**left, right, both, none**.

* **z-index** property allows you to control which box appears on top.

<br>

--- 

<br>

## Grid

1. define grid container element (parent) -> `display: grid`
2. set its column and row sizes -> `grid-template-columns` and `grid-template-rows`
3. place grid items (children) into the grid -> `grid-column` and `grid-row`

- children are only the direct descendants of the parent element
- _Note: column, float, clear, and vertical-align have no effect on a grid container._

### Terminology
1. grid container
2. grid item
3. grid line = The dividing lines that make up the structure of the grid.
4. grid track = column or row
5. grid cell = a single "unit" of the grid.
6. grid area = The total space surrounded by four grid lines. Can contain any number of cells.


<br>
<br>

---

## Layout Summary


* **`<div>` elements are often used as containing elements to group together sections of a page.**

* **Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning.**
* **The float property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width.)**
* **Pages can be fixed width or liquid (stretchy) layouts.**
* **Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).**
* **Grids help create professional and flexible designs.**
* **CSS Frameworks provide rules for common tasks.**
* **You can include multiple CSS files in one page.**

<br> 
<br>

You Can Read More About CSS Position, [HERE](https://css-tricks.com/almanac/properties/p/position/)
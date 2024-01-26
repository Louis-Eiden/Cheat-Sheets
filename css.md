# CSS Cheat Sheet

---
## **UNDER CONSTRUCTION**
---

## Table of Contents
- [Selectors](#selectors)
- [Properties](#properties)
- [Units](#units)
- [Box Model](#box-model)
- [Layout](#layout)
- [Typography](#typography)
- [Colors](#colors)
- [Backgrounds](#backgrounds)
- [Transitions and Animations](#transitions-and-animations)

## Selectors
- Element selector: `element`
- Class selector: `.class`
- ID selector: `#id`
- Attribute selector: `[attribute=value]`
- Pseudo-class selector: `:pseudo-class`
- Pseudo-element selector: `::pseudo-element`

## Pseudo-classes
- `:active`: Selects the active link
- `:checked`: Selects every checked element
- `:disabled`: Selects every disabled element
- `:empty`: Selects every element that has no children
- `:enabled`: Selects every enabled element
- `:first-child`: Selects the first child element
- `:first-of-type`: Selects the first element of its type
- `:focus`: Selects the element that has focus
- `:hover`: Selects the element that is being hovered
- `:in-range`: Selects input elements with a value within a specified range
- `:invalid`: Selects all invalid input elements
- `:lang(language)`: Selects every element with a lang attribute equal to language
- `:last-child`: Selects the last child element
- `:last-of-type`: Selects the last element of its type
- `:link`: Selects all unvisited links
- `:not(selector)`: Selects every element that is not a selector
- `:nth-child(n)`: Selects every element that is the nth child, regardless of type, of its parent
- `:nth-last-child(n)`: Selects every element that is the nth child, regardless of type, of its parent, counting from the last child
- `:nth-last-of-type(n)`: Selects every element that is the nth child, of a particular type, of its parent, counting from the last child
- `:nth-of-type(n)`: Selects every element that is the nth child, of a particular type, of its parent
- `:only-of-type`: Selects every element that is the only child of its parent, of a particular type
- `:only-child`: Selects every element that is the only child of its parent
- `:optional`: Selects input elements with no "required" attribute
- `:out-of-range`: Selects input elements with a value outside a specified range
- `:read-only`: Selects input elements with the "readonly" attribute specified
- `:read-write`: Selects input elements with the "readonly" attribute NOT specified
- `:required`: Selects input elements with the "required" attribute specified
- `:root`: Selects the document's root element
- `:target`: Selects the current active #hash-tagged URL
- `:valid`: Selects all valid input elements
- `:visited`: Selects all visited links

---

## Pseudo-elements
- `::after`: Insert something after the content of each selected element
- `::before`: Insert something before the content of each selected element
- `::first-letter`: Selects the first letter of each selected element
- `::first-line`: Selects the first line of each selected element
- `::selection`: Selects the portion of an element that is selected by a user

## Properties

### Box Model
- `margin`: Space outside the border
- `border`: Border around the element
- `padding`: Space between the content and the border
- `width`: Width of the content area
- `height`: Height of the content area

### Layout
- `display`: Element display type
- `position`: Element positioning
- `float`: Element floating
- `clear`: Clear floating elements
- `flexbox`: Flexible box layout
- `grid`: Grid layout

### Typography
- `font-family`: Font family
- `font-size`: Font size
- `font-weight`: Font weight
- `text-align`: Text alignment
- `text-decoration`: Text decoration
- `text-transform`: Text transformation
- `line-height`: Line height

### Colors
- `color`: Text color
- `background-color`: Background color
- `opacity`: Element opacity

### Backgrounds
- `background`: Background
- `background-color`: Background color
- `background-image`: Background image
- `background-repeat`: Background repeat
- `background-position`: Background position
- `background-size`: Background size
- `background-attachment`: Background attachment
- `background-clip`: Background clip
- `background-origin`: Background origin
- `background-blend-mode`: Background blend mode

### Transitions and Animations
- `transition-property`: Property to transition
- `transition-duration`: Transition duration
- `transition-timing-function`: Transition timing function
- `transition-delay`: Transition delay
- `animation-name`: Animation name
- `animation-duration`: Animation duration
- `animation-timing-function`: Animation timing function
- `animation-delay`: Animation delay
- `animation-iteration-count`: Animation iteration count
- `animation-direction`: Animation direction

### List
- `list-style-type`: List style type
- `list-style-position`: List style position
- `list-style-image`: List style image

### Table
- `border-collapse`: Border collapse
- `border-spacing`: Border spacing
- `caption-side`: Caption side
- `empty-cells`: Empty cells
- `table-layout`: Table layout

### Transform
- `transform`: Transform
- `transform-origin`: Transform origin
- `transform-style`: Transform style
- `perspective`: Perspective
- `perspective-origin`: Perspective origin
- `backface-visibility`: Backface visibility

### Visibility
- `visibility`: Visibility
- `overflow`: Overflow
- `overflow-x`: Overflow x-axis
- `overflow-y`: Overflow y-axis
- `clip`: Clip

### Interactivity
- `cursor`: Cursor
- `pointer-events`: Pointer events
- `resize`: Resize
- `user-select`: User select

### Box Sizing
- `box-sizing`: Box sizing

### Outline
- `outline`: Outline
- `outline-width`: Outline width
- `outline-style`: Outline style
- `outline-color`: Outline color
- `outline-offset`: Outline offset

### Border
- `border`: Border
- `border-width`: Border width
- `border-style`: Border style
- `border-color`: Border color
- `border-top`: Border top
- `border-top-width`: Border top width
- `border-top-style`: Border top style
- `border-top-color`: Border top color
- `border-right`: Border right
- `border-right-width`: Border right width
- `border-right-style`: Border right style
- `border-right-color`: Border right color
- `border-bottom`: Border bottom
- `border-bottom-width`: Border bottom width
- `border-bottom-style`: Border bottom style
- `border-bottom-color`: Border bottom color
- `border-left`: Border left
- `border-left-width`: Border left width
- `border-left-style`: Border left style
- `border-left-color`: Border left color
- `border-radius`: Border radius
- `border-top-left-radius`: Border top left radius
- `border-top-right-radius`: Border top right radius
- `border-bottom-right-radius`: Border bottom right radius
- `border-bottom-left-radius`: Border bottom left radius
- `border-image`: Border image
- `border-image-source`: Border image source
- `border-image-slice`: Border image slice
- `border-image-width`: Border image width
- `border-image-outset`: Border image outset
- `border-image-repeat`: Border image repeat

---

## Units
- `px`: Pixels
- `%`: Percentage
- `em`: Relative to the font-size of the element
- `rem`: Relative to the font-size of the root element
- `vh`: Relative to the viewport height
- `vw`: Relative to the viewport width

## Box Model
- `margin`: Space outside the border
- `border`: Border around the element
- `padding`: Space between the content and the border
- `width`: Width of the content area
- `height`: Height of the content area

## Layout
- `display`: Element display type (e.g., `block`, `inline`, `flex`)
- `position`: Element positioning (e.g., `static`, `relative`, `absolute`)
- `float`: Element floating (e.g., `left`, `right`)
- `clear`: Clear floating elements (e.g., `left`, `right`, `both`)
- `flexbox`: Flexible box layout
- `grid`: Grid layout

## Typography
- `font-family`: Font family
- `font-size`: Font size
- `font-weight`: Font weight
- `text-align`: Text alignment
- `text-decoration`: Text decoration (e.g., `underline`, `line-through`)
- `text-transform`: Text transformation (e.g., `uppercase`, `lowercase`)
- `line-height`: Line height

## Colors
- `color`: Text color
- `background-color`: Background color
- `opacity`: Element opacity

## Backgrounds
- `background-color`: Background color
- `background-image`: Background image
- `background-repeat`: Background repeat (e.g., `repeat`, `no-repeat`)
- `background-position`: Background position (e.g., `top left`, `center center`)
- `background-size`: Background size (e.g., `cover`, `contain`)

## Transitions and Animations
- `transition-property`: Property to transition
- `transition-duration`: Transition duration
- `transition-timing-function`: Transition timing function
- `transition-delay`: Transition delay
- `animation-name`: Animation name
- `animation-duration`: Animation duration
- `animation-timing-function`: Animation timing function
- `animation-delay`: Animation delay
- `animation-iteration-count`: Animation iteration count
- `animation-direction`: Animation direction


## Tricks and Tips

### calculate percentage from px
```css
width: calc(100% - 100px);
```

pixel / container size * 100 = %

### center element horizontally
```css
margin: 0 auto;
```

### center element vertically
```css
position: absolute;
top: 50%;
transform: translateY(-50%);
```

### center element horizontally and vertically
```css
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
```

### center element horizontally and vertically with flexbox
```css
display: flex;
justify-content: center;
align-items: center;
```

### center element horizontally and vertically with grid
```css
display: grid;
place-items: center;
```

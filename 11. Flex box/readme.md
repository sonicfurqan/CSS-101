# flexbox

modern grid style to create layouts

To create a flexbox there is the hierarchy that needs to be followed

by making parent element as flex container all the elements inside the container becomes flex item

To make parent element flex box define display property as flex 
```css 
    div{ 
        display: flex; 
    }
    /*or*/
    div{
        display:inline-flex;
    }
``` 

hereby making div as flex all the inner elements becomes flex item

# display:flex;

by making display as flex all the inner element becomes flex item i.e

this will affect how elements behave

all the elements will now be adjacent to each other by default and occupy only content width

all the elements will occupy height that is equal to the highest hight of one element

container element has the following properties

### flex-wrap

using flex wrap we can control how the elements behave when resizing

it accepts following properties

nowrap : by default its no wrap. behaviour would be when the display size is reduced then the element will occupy the width that is needed for content and stop 

wrap : behaviour would be when the display size is reduced then element will jump to next light to fit in

```css
div{ 
    display: flex; 
    flex-wrap:wrap;
}
```

### flex-direction

using flex-direction we can control the alignment of elements 

either horizontal or vertical

row : by default its row. 
behaviour would be each element will align adjacent to each other.
element with no height will occupy height equal to the highest elements height in container.
when weight is reduced element will reduce the width to a minimum to content that it can hold
the main axis is horizontal
cross axis is vertical

column: this makes the alignment vertical
behavour would be each element will align below to each other.
element with no width will occupy the width equal to the highest elements width in the container.
when width is reduced element will reduce width to minimum irrespective of the content
main axis is vertical
cross axis is horizontal

### align-items - position on cross axis

using align-items we can align-items.
for the horizontal direction it aligns item top to bottom
for the vertical direction it aligns item left to right

stretch : by default. items are aligned normally to the base

center : items are aligned to centre

flex-start : items are aligned to the baseline of container for horizontal
items are aligned to the left side for vertical 

flex-end : items are aligned to the top line of container for horizontal
items are aligned to right side for vertical 

baseline : items are aligned to contents baseline

### justify-content - position on main axis

using align items we can align items.
for the horizontal direction, it aligns item left to right
for vertical direction it aligns item top to bottom

stretch : by default. items are aligned normally to the base

center : items are aligned to center

flex-start : items are aligned to base line of container for horizontal
items are aligned to left side for vertical 

flex-end : items are aligned to top line of container for horizontal
items are aligned to right side for vertical 

### align-content:

using align content we can postion elemets

space-between: it aligns elements to far left and far right base on window size 

# Flex item

elements under the container element that has a position as flex applied are flex item

properties of flex item

### order

using order items can be positioned in axis it works similar to z-index but not same 

order takes integer value - to +.

0 is the default.  - value makes element move to start and + makes the elements move to end 

### align-self

align-slef is similar to align-items. it takes same values as align-item.
The difference is it affects only one element that is under the flex container.


### flex-grow

using flex grow we can allocate the space to the element that it can occupy. flex grow takes a positive integer as input

example

if there are 3 elements and we provide flex-grow:1 to all elements then width is divided in 3 equal parts with elements

if there are 3 elements and we provide flex-grow:1 to 2 elements and flex-grow:2 to one element then width is divided into 4 parts and 2 parts are given to one and 1 1 to each with 1 value

Note: if there are no elements in row/column then width is not divided as no element is present to divided and allocate space

### flex-shrink

flex-shrink is opposite to flex grow. It accepts positive integer value default is 1, it allows element to shrink if it is set to 0 then it doesn't allow to shrink.

it controls the shrinking of element


### flex-basis

using this we can  set width for horizontal direction and height for the vertical direction
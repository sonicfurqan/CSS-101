# flex box

    mordern grid style to create layouts

    To create a flex box there is hirarchy that needs to be followed

    by making parent element as flex container all the elements inside the contaner becomes flex item

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

    here by making div as flex all the inner elemens becomes flext item

# display:flex;

    by making diaplay as flex all the inner element becomes flex item i.e

    this will effect how elements are behaved

    all the elements will now be adjesent to each other by default and occopy only content width

    all the elements will occupy height that is equal to highest hight of one element

    container element has following properties

## flex-wrap

    using flex wrap we can control how the elemetns bahave when resizing

    it accepts following propertes

    nowrap : by default its no wrap. behaviour would be when the display size is reduced then element will occpy the width that is needed for content and stop 

    wrap : behaviour would be when the display size is reduced then element will jump to next light to fit in

```css
div{ 
    display: flex; 
    flex-wrap:wrap;
}
```

## flex-direction

    usint flex direction we can control the aligenment of elements 

    either horizontal or vertical

    row : by default its row. 
    behavor would be each element will align adjesent to each other.
    element with no height will occupy height equal to highest elements heigth in conteiner.
    when widht is reduced element will reduce width to minimum to content that it can hold
    main axis is horizontal
    cross axis is vertical

    column : this makes the alightnment vertical
    behavour would be each eleent will align below to each other.
    element with no width will occupy the width equal to highest eleements width in container.
    when width is reduced element will reduce width to minimum irrespective of content
    main axis is vertical
    cross axis is horizontal

## align-items - position on cross axis

    using align items we can align items.
    for horizontal direction it aligns item top to bottom
    for vertical direction it aligns item left to right

    stretch : by default. items are aligned normaly to the base

    center : items are aligned to center

    flex-start : items are aligned to base line of container for horizontal
    items are aligned to left side for vertical 

    flex-end : items are aligned to top line of container for horizontal
    items are aligned to right side for vertical 

    baseline : items are aligned to contents baseline

## justify-content - position on main axis

    using align items we can align items.
    for horizontal direction it aligns item left to right
    for vertical direction it aligns item top to bottom

    stretch : by default. items are aligned normaly to the base

    center : items are aligned to center

    flex-start : items are aligned to base line of container for horizontal
    items are aligned to left side for vertical 

    flex-end : items are aligned to top line of container for horizontal
    items are aligned to right side for vertical 

## align-content:

    using align content we can postion elemets

    space-between: it aligns elements to far left and far right base on window size 

# Flex item

    elements under the container element that has position as flex applied are flex item

    porperties of flex item

## order

    using order items can be positioned in axis it works similare to z-index but not same 

    order takes integer value - to +.

    0 is default.  - value makes element move to starting and + makes the elements move to end 

## align-self

    align-slef is simmilar to align-items. it takes same values as align-item.
    The diffrence is it effects only one element that is under the flex container.


## flex-grow

    using flex grow we can allocate the space to element that it can occupy . flex grow takes positive integer as input

    example

    if there are 3 elements and we provide flex-grow:1 to all elements then width is devided in 3 eqal partes with elements

    if there are 3 elements and we provide flex-grow:1 to 2 elements and flex-grow:2 to one element then width is devided into 4 partes and 2 partes are given to one and 1 1 to each with 1 value

    Note: if there are no elements in row/coloum then width is not deved as no element is present to devied and allocate space

## flex-shrink

    flex-shrink is opposite to flex grow. It accepts positive integer value default is 1, it allwows element to shrink if it is set to 0 then it doesnt allow to shrink.

    it controls the shrinking of element


## flex-basis

    using this we can  set width for horizontal direction and height for vertical direction
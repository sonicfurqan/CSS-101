# Sizing reference

to apply the size CSS use 3 different reference point


1. Absolute: values that are defined by "px" are considered as absolute i.e the size doesn't change irrespective to page size font size

2. viewport: values that are defined by vh,vw changes the sizing based on the relative change of window height and width

3. font-dependet : values that are defined by rem,em changes the sizing based on the relative change of  font size

# Pixel (px)

exact pixel value that is assigned to value for it to occupy

```css
div{
    height:10px;
}
```

# Percentage (%)

Specify that element can occupy the defined percentage available to it from the parent element

Note:

1. When % is applied to position fixed element then the reference is viewport

2. When % is applied to position absolute/static/relative element then the reference is the nearest parent element that has a position applied to it

# em (em)

1 em is 16 px 
```css
div{

    font-size:1em; /*= 16px*/

}
```

# rem (rem)

this refers to the default font value of browser when calculating pixels for reference
```css
div{

    font-size:1rem; /*= 16px if browser font settings is medium*/

}
```


# vh,vw

    with these parameters, sizing can be defined in reference to viewport 


```css
div{
    height:50vh;/*this implies  height to be equal to 50% of display area*/
    width:80vw;/*this implies width  to be equal to 80% of display area*/
}
```
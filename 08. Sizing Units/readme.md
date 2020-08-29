# Sizing refrence

    to appy the size css use 3 diffrent refrence point


1. Absolute : values that are defined by "px" are considred as absolute i.e the size doesnt change ir respective to page size font size

2. viewport : values that are defined by vh,vw changes the sizing baased on relatve change of window height and width

3. font-dependet : values that are defined by rem,em changes the sizing based on relative change of  font size

# Pixel (px)

    exact pixel value that is assigned to value for it to occupy

```css
div{
    height:10px;
}
```

# Percentage (%)

    Specify that element can occupy the defined percentage avilabel to it from parent element

    Note:
    1. When % is applied to position fixed element then refence is view port

    2.1. When % is applied to position absolute/static/relative element then refence is nearest parent element that has postion applied to it

# em (em)

    1 em is 16 px 
```css
div{

    font-size:1em; /*= 16px*/

}
```

# rem (rem)

    this refres to the default font value of browser when calculating pixels for refrence
```css
div{

    font-size:1rem; /*= 16px if browser font settings is medium*/

}
```


# vh,vw

    with this parameters sizing can be defined in refrence to view port 


```css
div{
    height:50vh;/*this implies  height to be equal to 50% of display area*/
    width:80vw;/*this implies width  to be equal to 80% of display area*/
}
```
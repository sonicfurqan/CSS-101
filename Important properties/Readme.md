# box-sizing

    this property controls how the width and height is calculated of element
    
    1. Default is "content-box" : when height and width is set of element it actually applies to elements content doesn't include margin and border size

    2. "border-box" : when height and width is set of the element it actually applies to elements including margin and border size

```css
div{
    box-sizing:border-box;
}
```

 # list-style

    this property controls how ul,li list is displayed 

    1. none : removes the bullet that is shown on li item

```css
ul{
    list-style:none;
}
```

# text-decoration

    this properties control the text behaviour example underlining a text or struckthrough a text
```css
a{
    text-decoration:none;
}
```

# filter

    this property allows adding effect to background properties example it can apply blur,grayscale effect

```css
div{
    background:black;
    height:10px;
    filter:blur(20px);
}
```

# Margin: auto

    by assigning auto to margin it centres the element in middle. This will work for block-level element

```css
div{
    display:block;
    margin:auto;
}
```
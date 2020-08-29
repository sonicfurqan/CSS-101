# box-sizing

    this propertie controles how the widht and height is calculuated of element
    
    1. Default is "content-box" : when height and widht is set of element it acually applies to elemetns content doesnt include margin and border size

    2. "border-box" : when height and widht is set of element it acually applies to elemetns including margin and border size

```css
div{
    box-sizing:border-box;
}
```

 # list-style

    this propertie controles how ul,li list are displayed 

    1. none : removes the bullet that are shown on li item

```css
ul{
    list-style:none;
}
```

# text-decoration

    this propeties controles the text behavior example underlineing a text or stricktrhoug a text
```css
a{
    text-decoration:none;
}
```

# filter

    this proptie allows adding affect to background propertie example it can apply blur,grayscale affect

```css
div{
    background:black;
    height:10px;
    filter:blur(20px);
}
```

# Margin : auto

    by assiging auto to margin it centers the element in middile. This will work for block level element

```css
div{
    display:block;
    margin:auto;
}
```
## transform

using transform property we can change  an element 

#### rotateZ()

Using rotatez() function element can be rotated along the y-axis
function take 1 parameter it can be deg,px,rem,% that defines the rotateing angle

```css
div{
    transform:rotateZ(45deg);
}
```

#### tanslateX()

using translatex() function  element can be moved along its x-axis
function takes 1 parameters it can be rem,px that defines how it much it is moved

```css
div{
    transform:translateX(20px);
}
```

#### skewX()

using skewx() function element can be  angled like italic along its x-azis
function take 1 parameter it can be deg that defines the angle of skewnes

```css
div{
    transform:skewX(20deg);
}
```

#### scaleX()

using scaleX() function element can be scaled by the width
function take parameters it can be integer values that defines the the factor by which the element is scaled

```css
div{
    transform:scaleX(2);
}
```


## transform-origin

using this property we can define  the pivot point from whare transform will orgin 
it takes default value like left,right,center
and also the px,rem,%

```css
div{
    transform-origin:top right;
}

```




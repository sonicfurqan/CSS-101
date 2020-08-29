# view port meta tag

    to make website responseive to mobile screen meta tag is needed to be addedd to html

    with the help of viewport meta it helps the website to be aware of the display size of video. Is it on small device like mobile or big screen like monitor
    
    meta tag has 2 properties

    name : this should be equal to viewport

    content : this is comma seprated field that has following values

    width=device-width : by setting this value it maps the device view width to css width

    inital-scale=1.0 : tis defines the default zoom level.

    user-scalable=yes : if yes then user can zoom into page and if no it doesnt allow user to zoom 

```html

<meta name="viewport" content="width=device-width,inital-scale=1.0"></meta>
```


# media query

    using meda query styles can be defined for diffrent conditions
    example if device width is decresed on increased
    
    media query takes input of one propertie that acts as if condition

    inside meda query condition , css selectior and declariton  can be defined


    If using mobile first development then media query with min-width will take affect on large device

    If ussing web first development then media query with max-width will take affect on small device

```css
@media (min-width:320px){
    div{
        font-size:48px;
    }
}

@media (max-width:320px){
    div{
        font-size:48px;
    }
}

```
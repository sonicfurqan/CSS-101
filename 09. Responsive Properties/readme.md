# viewport meta tag

to make website responsive to mobile screen meta tag is needed to be added to html

with the help of viewport meta it helps the website to be aware of the display size of video. Is it on small devices like mobile or big screen like monitor

meta tag has 2 properties

name : this should be equal to viewport

content: this is the comma separated field that has the following values

width=device-width : by setting this value it maps the device view width to css width

inital-scale=1.0 : tis defines the default zoom level.

user-scalable=yes : if yes then the user can zoom into page and if no it doesn't allow user to zoom 

```html

<meta name="viewport" content="width=device-width,inital-scale=1.0"></meta>
```


# media query

using media query styles can be defined for different conditions
example if the device width is decreased on increased

media query takes input of one property that acts as if the condition

inside media query condition , css selector and declaration  can be defined


If using mobile-first development then media query with min-width will take effect on large device

If using web first development then media query with max-width will take effect on small device

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
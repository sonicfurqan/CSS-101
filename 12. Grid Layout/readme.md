# Css Grid

Using display grid layouts can be designed for positioning elements
It also follows hierarchy like flex box.making parent dive as display gird makes all child elements grid elements of container

note: grid default have horizontal flow it places element adjacent to each other and based on column configuration extra elements are pushed in new row

it can be overridden by grid-auto-flow: column; then the elements that doesn't fit the grid are added as new columns 

by using auto-fill variable in template column/row elements are positioned according to screen size in grid

by using auto-fit variable in template column/row elements are positioned according to screen size in grid and also centred

```css
div{
    display:grid;
}
```

### grid-auto-row/colum

using this property we can add default minimum height/width of element added to new row or column

### grid-template-coloum

using this property we can define the number of columns and there respective width 

it accepts n values separated by space, each value will represent the number of columns 

it can accept new value like px,em. It is a fraction fr. By defining size fr it splits the space between elements 

if auto is set as last value then element takes the value that is remaining after the split

```css
div{
    display:grid;
    grid-template-columns:10% 100px 1fr;
}
```

### grid-template-rows

using this property we can define the height of row in grid

it accepts n value separated by space,each value will represent the number of rows that it implicitly assign the height

Note:if row dimension are defined more then the elements in container extra space is occupied on the layout

```css
div{
    display:gird;
    grid-template-rows:10px 2rem;
}
```

### grid-row/column-gap : grid-gap

using this property we can define the space between the rows and column of the grid template

```css
div{
    grid-column-gap:20px;
    grid-row-gap:10px;
}
p{
    grid-gap:10px 10px;
}
```
### grid-template-areas :

using this property you can define the area name for each row or column that is defined in a template

note: rows and columns should match with are names defined

```css
div{
    display:grid;
    grid-template-column:10% 10%;
    grid-template-row:10% 10% 10%;
    grid-template-areas:"header header"
    "main main"
    "footer footer";

}
```

# Align Container

### justify-content

this property aligns the container in its respective element size example:start,end,center
using this it aligns  in a horizontal direction

```css
div{
    display:grid;
    justify-content:center
}
```


### align-content

this property aligns the container in its respective element size example:start,end,center
using this it aligns  in the verticle direction

```css
div{
    display:grid;
    align-content:center
}
```

# Align Items

### justify-items

this property aligns the elements in there respective position in grid example:start,end,center
using this it aligns item in the horizontal direction

```css
div{
    display:grid;
    justify-items:center
}
```
### align-items

this property aligns the elements in their respective position in grid example:start,end,center
using this it aligns item in the verticle direction

```css
div{
    display:grid;
    align-items:center
}
```

# Grid elements

when grid is created and grid template rows and columns properties are set it creates rows and columns with respective numbers starting from 1,2 and so on

### grid-column-start /grid-column

using this property we can set the elements position where it starts in the grid by column number

### grid-column-end  /grid-column

using this property we can set the position of the element where it ends in grid by column number

it also accepts the key word span using that we can define that element should occupy next n column

Note: if the value is defined -1  it will occupy the whole row

```css

div{
    grid-column-start:2;
    grid-column-end :span 4;
}
```

### grid-row-start / grid-row

using this property we can set the position of the element where it starts in grid by row number

### grid-row-end  / grid-row

using this property we can set the position of the element where it ends in grid by row number

    
```css

div{
    grid-row-start:2;
    grid-row-end :4;
}
```

### grid-area

using this element can be position in area that is defined using property gird template areas in container gird

```css
div{
    grid-area:footer;
}
```



### justify-self

this property aligns the element in its respective position in grid example:start,end,center
using this it aligns item in the horizontal direction

```css
div{
    justify-self:center
}
```
### align-self

this property aligns the element in its respective position in grid example:start,end,center
using this it aligns item in the verticle direction

```css
div{
    align-self:center
}
```


4,30,000
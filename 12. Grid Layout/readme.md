# Css Grid

    Using display grid layouts can be desgined for positioning elements
    It also follows hirarchy like flex box.making parent dive as dispaly gird makes all child elements grid elements of continer

    note: grid defualt have horizontal flow it places element adjecent to each other and based on coloum configurtaion extra elements are pushed in new row

    it can be overridden by grid-auto-flow:column; then the elements that doesnt fit the grid are added as new columns 

    by using auto-fill variable in template column/row elements are postioned according to screen size in grid

    by using auto-fit variable in template column/row elements are postioned according to screen size in grid and also centered

```css
div{
    display:grid;
}
```

## grid-auto-row/colum

    using this property we can add default minimum height/width of element addedd to new row or column

## grid-template-coloum

    using this proeperty we can define the number of coloums and there respective width 

    it accepts n values seprated by space, each value will represent the number of coloumns 

    it can accept new value like px,em. It is fraction fr. By defineg size fr it splits the space between elements 

    if auto is set as last value then element takes the value that is remaing after the split

```css
div{
    display:grid;
    grid-template-columns:10% 100px 1fr;
}
```

## grid-template-rows

    using this property we can define the height of row in grid

    it accepts n value seprated by space,each value will represent the number of rows that it implcitly assign the height

    Note:if row dimintion are defined more then the elements in container extra space is occupied on layout

```css
div{
    display:gird;
    grid-template-rows:10px 2rem;
}
```

# grid-row/column-gap : grid-gap

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
# grid-template-areas :

    using ths property you can define the area name for each row or column that is defined in template

    note:rows and coloumns should match with are names defined

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

# align-container

# justify-content

   this property aligns the container in its respective element size example:start,end,center
   using this it aligns  in horizontal direction

```css
div{
    display:grid;
    justify-content:center
}
```


# align-content

   this property aligns the container in its respective element size example:start,end,center
   using this it aligns  in verticle direction

```css
div{
    display:grid;
    align-content:center
}
```

# align items

## justify-items

    this property aligns the elements in there respective position in grid example:start,end,center
    using this it aligns item in horizontal direction

```css
div{
    display:grid;
    justify-items:center
}
```
## align-items

    this property aligns the elements in there respective position in grid example:start,end,center
    using this it aligns item in verticle direction

```css
div{
    display:grid;
    align-items:center
}
```

# Grid elements

    when grid is created and grid template rows and columns propertues are set it creates rows and colums with respective numbers starting from 1,2 and so on

## grid-column-start /grid-column

    using this proterty we can set the elements postion where it starts in grid by column number

## grid-column-end  /grid-column

    using this proterty we can set the elements postion where it ends in grid by column number

    it also accepts the key workd span using that we can define that element should occupy next n colum

    Note: if value is defined -1  it will occupy the whole row

```css

div{
    grid-column-start:2;
    grid-column-end :span 4;
}
```

## grid-row-start / grid-row

    using this proterty we can set the elements postion where it starts in grid by row number

 ## grid-row-end  / grid-row

    using this proterty we can set the elements postion where it ends in grid by row number

    
```css

div{
    grid-row-start:2;
    grid-row-end :4;
}
```

# grid-area

    using this element can be psosition in area that is defined using property gird template areas in container gird

```css
div{
    grid-area:footer;
}
```



## justify-self

    this property aligns the element in its respective position in grid example:start,end,center
    using this it aligns item in horizontal direction

```css
div{
    justify-self:center
}
```
## align-self

    this property aligns the element in its respective position in grid example:start,end,center
    using this it aligns item in verticle direction

```css
div{
    align-self:center
}
```
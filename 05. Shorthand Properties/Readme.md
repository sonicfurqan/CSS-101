# Shorthand properties

Combining multiple properties of the same type and writing in single properties.

## Example

1. For Border :
```css
div{
    border-width:2px;
    border-style:solid;
    border-color:black;
}
```
can be wrriten as 
```css
div{
    border:2px solid black;
}
```
Order of values doesn't matter as each value is of different type

2. For Margin :
```css
div{
    margin-top:2px;
    margin-right:3px;
    margin-bottom:4px;
    margin-left:5px;
}
```
can be wrritten as
```css
div{
    margin:2px 3px 4px 5px;
}
```
order of value matters as all the value of the same type

3. for grid-column
```css
div{
    grid-column-start:1;
    grid-column-end: span 1;
}
```
can be written as

```css
div{
    grid-column:1 / span 1;
}
```

3. for grid-row
```css
div{
    grid-row-start:1;
    grid-row-end: 2;
}
```
can be written as

```css
div{
    grid-row:1 / 2;
}
```
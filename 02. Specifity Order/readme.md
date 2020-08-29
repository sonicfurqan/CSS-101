# Styling order/precedence 

Order of Style applied to an element if there are multiple styles in effect


1. Inline Style : Highest order this will over write all styling
```html
<div style="color:redl"></div>
```

2. Id Selector : priority is given to css declartions provided using id selector after ininle style
```css
#id-selector{
    color:red;
}
```

2. Class Selector : priority is given to css declartions provided using Class selector after inline style
```css
.class-selector{
    color:red;
}
```

4. Tag Selector : priority is given to css declartions provided using Tag selector after Class style
```css
div{
    color:red;
}
```

5. Inherited Styling : if parent element has css declation defined and child element is not overriting it using selectors then inherited styling is given priority.
```css
body{
    color:red;
}
```

```html
<body>
    <div>
        all text under body inherits color red unless over ridded
    </div>
<body>
```
# Types to add CSS style

1. Inline Styling : Adding style to html element directly by using style tag
```html
    <div style="color:red;">
        red color text
    </div>
```

2. Styling with Selector:Adding style to html element using id/class/tag of element
```css
#id-of-element{
    color:red;
}
.class-for-elements{
    background:black;
}
div{
    border-style:groove;
     border-color:green;
}
```

```html
    <div>
        tag style
    </div>
    <div id="id-of-element">
        id styleing
    </div>
    <div class="class-for-elements">
        class styling
    </div>
```

3. Global Styling: Adding style to all elements of HTML using *
```css
*{
    font-family: sans-serif;
}
```

```html
    <div>
        custom font set for all web page 
    </div>
```

4. Styling with Attributes: Add styleing to element based on tag attribute
```css
[disabled]{
    font-size:large;
}
```
```html
    <button disabled>
        all elements with disalbed tag 
    </button>
```


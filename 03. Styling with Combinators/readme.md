# Css Combinators

    Adding style child  elements/element using combination of class/id/tag 

1. Adjacent Sibling ( + ): Applyies css to adjesent element of parent selector specified. Only direct sibling gets css properties i.e in following example p tag should be defined next to h2 tag
```css
h2 + p{
    color:red;
}
```
```html
<div>
    <h2>parent element</hr>
    <p>css applied</p>
    <h3>elemnt</h3>
    <p>css not applied</p>
</div>
```

2. General Sibling ( ~ ): Applyies css to adjesent elements of parent selector specified. all sibling gets css properties i.e in following example p tag can be defined in same level as h2 tag
```css
h2 ~ p{
    color:red;
}
```
```html
<div>
    <h2>parent element</hr>
    <p>css applied</p>
    <h3>elemnt</h3>
    <p>css  applied</p>
</div>
```

3. Child Elements ( > ): Applyies css to child elements of parent selector spceifed. all child elements which are defined bellow one level gets css properties i.e in following example all p tag elements get css propertes that are only defined directly under div
```css
div ~ p{
    color:red;
}
```
```html
<div>
    <h2>parent element</hr>
    <p>css applied</p>
    <h3>elemnt</h3>
    <span>
        <p>css not applied</p>
    </span>
    <p>css  applied</p>
</div>
```

4. Decendent Elements ( "blank" ) : Applyies css to all child elements of parent selector spceifed. all child elements which are defined bellow parent selector gets css properties i.e in following example all p tag elements get css propertes that are  defined  under div
```css
div  p{
    color:red;
}
```
```html
<div>
    <h2>parent element</hr>
    <p>css applied</p>
    <h3>elemnt</h3>
    <span>
        <p>css  applied</p>
    </span>
    <p>css  applied</p>
</div>
```
# CSS Combinators

    Adding style child  elements/element using combination of class/id/tag 

1. Adjacent Sibling ( + ): Applies CSS to adjacent element of parent selector specified. Only direct sibling gets CSS properties i.e in following example p tag should be defined next to h2 tag
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

2. General Sibling ( ~ ): Applies CSS to adjacent elements of parent selector specified. all sibling gets CSS properties i.e in following example p tag can be defined in the same level as h2 tag
```css
h2 ~ p{
    colour:red;
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

3. Child Elements ( > ): Applies CSS to child elements of parent selector specified. all child elements which are defined bellow one level get CSS properties i.e in following example all p tag elements get CSS properties that are only defined directly under div
```css
div > p{
    colour:red;
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

4. Decedent Elements ( "blank" ): Applies CSS to all child elements of parent selector specified. all child elements which are defined bellow parent selector get CSS properties i.e in following example all p tag elements get CSS properties that are  defined  under div
```css
div  p{
    colour:red;
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
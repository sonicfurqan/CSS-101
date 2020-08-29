# Pseudo-classes

pseudo-classes allow styling of an element in different state example on hover or on focus

## Types of a pseudo selector

1. State (:) -> defined after the colon ":" for targeting perticular state of element
```css
a:hover{
    color:red;
    font-weight:bold;
}
```

2. Element (::) -> deifined after the double colon "::" for targeting content of element
```css
p::first-letter{
    font-weight:bold;
}


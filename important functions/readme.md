# calc

    Useing this function calculate height/width dynamically
```css
#div1 {
  position: absolute;
  left: 50px;
  width: calc(100% - 100px);
  border: 1px solid black;
  background-color: yellow;
  padding: 5px;
  text-align: center;
}
```

# :not()

    using this pseudo selector you can target an element without the defined call/id

```css
:not(p) {
  background: #ff0000;
}

```
# linear-gradient

    using this on background properties you can create a gradient of colours
    it take multiple parameters as input
    1. first is angle of a gradient in deg
    2. then it follows the sequence of colors or images desired for gradient
    3. along with color/image percentage of the gradient can be defined in 

```css
div{
    background:linear-gradient(180deg,red 60%,black );
}

```

# repeat

  using this function we can repeat the specified value the number of times defined

  it takes 2 parameters
  first is the number of times it needs to repeat
  second is a value that it needs to repeat

```css

div{
  grid-template-column: repeat(10,20%);
}

```

# minmax

  using this we can setup the minimum and maximum the value using one line

  it accepts 2 parameters
  first defines the minimum value the element can occupy
  the second defines the maximum value the element can occupy

```css
div{
  grid-template-column: minmax(10%,20%);
}

```


# fit-content()

  using this function takes one parameter that is default size similar to min-width, it is used in grid layout

```css
  div{
    grid-template-row:fit-content(8rem);
  }

```
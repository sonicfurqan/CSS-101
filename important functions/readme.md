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

    using this sudo selector you can taget an element without the defined call/id

```css
:not(p) {
  background: #ff0000;
}

```
# linear-gradient

    using this on bacground propertie you can create a gradient of colors
    it take multiple parameters as input
    1. first is angle of gradient in deg
    2. then it follows the sequence of colors or images desried for gradient
    3. along with color/image percentage of gradient can be defined in 

```css
div{
    background:linear-gradient(180deg,red 60%,black );
}

```

# repeat

  using this funtion we can repeat the specified value the number of times defined

  it take 2 parameters
  first is number of times it needs to repeat
  second is value that it needs to repeat

```css

div{
  grid-template-column: repeat(10,20%);
}

```

# minmax

  using this we can setup the minium and maximum the value using one line

  it accepts 2 paramenters
  first defines the minimum value the element can occupy
  second defines the maximum value the element can occupy

```css
div{
  grid-template-column: minmax(10%,20%);
}

```


# fit-content()

  using this function it takes one parameters that is default size simmiler to min-width, it is used in grid layout

```css
  div{
    grid-template-row:fit-content(8rem);
  }

```
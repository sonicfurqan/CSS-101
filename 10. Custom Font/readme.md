# custom font using local

a custom font can be added to css using font-face attribute by using local file.

@font-face requires 2 attributes

font-family: font-family name that you want to give 

src : location of font file

font-weight : using this property you can differentiate font-weight

example
```css
@font-face{
    font-family:"custom-name";
    src:url('filename.ttf');
}

div{
    font-family:"custom-name";
}

```
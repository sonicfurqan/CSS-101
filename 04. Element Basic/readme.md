# CSS Box module
    
Every element in CSS is interpreted as a box that has the following basic properties


1. Height: Verticle space occupied by element on the webpage
    
2. Width: Horizontal space occupied by element on the webpage

3. Padding: Internal space i.e between the content of element and border 

4. border: outline of the element 

5. margin: extra space between the current element and other elements that are its siblings

6. display: controls the behaviour of element

7. colour: controls the text colour 

8. background-colour: controls the background-colour

9. background-image : set background image using "URL()" 

10. background-repeat: control the repentance of image posible values.
    
    no-repate,y-repeat,x-repeat

11. background-size: can set width and height and it also accepts the following values

    cover: image is adjected to fit inside container .it is automatically cropped

    contain: image is adjected in the container so that it is fully visible without cropping

12. background-position: background-position has 3 different sets of values that it can take

    if numbers in a pixel is provided then image moves by respective pixel

    if numbers in percentage are provided then the image is cropped that is not visible

    and it also accepts the following values

    centre: image is centred in the container

    left top: image is aligned to by left and top and bottom and right is cropped 
    combination of left, top,bottom, right works as well

Note: height and width properties only sets the height for element content this will not include values of padding/margin/border they are added extra to the element


## Margin Collapsing

If 2 elements that are siblings to each other and have margins.
Then the larger margin will take precedence and only that margin properties will come into effect



## Display types

1. Block: occupies full width by default

2. Inline : Occupy width that is equal to content. Margin/Padding (Top and Bottom)  doesn't apply to an inline element

3. none: Removes an element from display yet keeps it in HTML

4. inline-block: it is a mix of both block and inline i.e element will only occupy width that it requires and we can set margin/padding to an element
# Css Box module
    
    Every element in css is intrepreted as box that has following basic properties


1. Height : Verticle space occupied by element on webpage
    
2. Width : Horizontal space occupied by element on webpage

3. Padding : Internal space i.e between content of element and border 

4. border : outline of element 

5. margin : extra spece between current element and other element that are its siblings

6. display : controles behavior of element

7. color : controls the text color 

8. background-color : controls the background color

9. background-image : set background image using "url()" 

9.1. background-repeat : control the repetence of image
    
                        posible values . no-repate,y-repeat,x-repeat

9.2. background-size : can set width and height and it also accepts following values

                        cover: image is adjected to fit inside contaner .it is automaticaly croped

                        contain: image is adjected in container so that it is fully visible without croping

9.3. background-position : background positon has 3 diiffrent set of values that it can take

                        if numbers in pixel is provided then image moves by reppectie pixel

                        if numbers in percentage is provided then image is croped that is not visible

                        and it also accepts following values

                        center : image is centerd in container

                        left top : image is aligned to by left and top and bottom and right is croped 
                                    combination of left,top,bottom,right works as well

Note:height and width popertie only sets height for element content this will not include values of padding/margin/border they are added extra to the element


## Margin Collapsing

    If 2 elements that are siblings to each other and have margins.
    Then the margin that is larger will take precendence and only that margin properties will come into affect



## Display types

1. Block : occupys full width by defult

2. Inline : Occupys width that is equal to content . Margin/Padding (Top and Bottom)  doesnt apply to inline element

3. none : Removes element from display yet keeps it in html

4. inline-block : it is mix of both block and inline i.e element will only occupy width that it reqires and we can set margin/padding to element
# positioning context 

when setting top,bottom,left,right properties on an element it positions itself relative to a context

1. view port : visible view of the window

2. html : whole html document

3. element : initial position of element by default



# position types

1. Static: positioning context is viewport i.e relative to the visible window. Takes the element out of document flow

2. absolute: if parent element doesn't have display type applied then the position context will be html i.e relative to full html document.If the parent element has a display type applied example relative then position context will be relative to the parent element. Takes the element out of document flow

3. relative: position contact is the element itself i.e it is relative to the position where it initially recedes in the document flow. doesnt take the element out of document flow.

4. sticky: it is a combination of fixed and relative.postion context is viewport. element doesn't change position unless it reaches viewport relative position it sticks to positon and sticky position is relived when element leaves viewport i.e its parent content box is removed from the view port

5. fixed: it makes the element to be fixed at the position defined by top,bottom,left,right,. this makes the element relative to viewport


# positioning  properties

1. top : position on  y axis 

2. bottom : position on  y axis 

3. left : position on  x axis 

4. right: position on  x axis 

5. z-index  : position on  z axis 
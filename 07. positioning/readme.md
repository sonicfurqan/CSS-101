# positioning  properties

1. top : position on  y axis 

2. bottom : position on  y axis 

3. left : position on  x axis 

4. right: position on  x axis 

5. z-index	: position on  z axis 


# positioning context 

	when setting top,bottom,left,right properties on an element it positions itself relative to context

1. view port : visible view of window

2. html : whole html document

3. element : initial postion of element by default



# position types

1. Static: positioning context is view port i.e relative to visible window. Takes the element out of docuemnt flow

2. absolute : if parent element doesnt have display type applyied then the posiotion context will be html i.e relative to full html docuemnt .If parent element has display type aplied example relative then position context will be relative to parent element. Takes the element out of document flow

3. relative : postion contect is element itselft i.e it is realtavie to postion where it initaly recides in docuemnt flow.doenst take the element out of docuemnt flow.

4. sticky : it is combination of fixed and relative.postion context is view port. element doesnt change postion unless it reaches view port relative postion it stickes to positon and stcky postion is relvied when element leves view port i.e its parent content box is removed from view port

5. fixed: it makes the element to be fixed at position defined by top,bottom,left,right,. this makes the element relative to view port
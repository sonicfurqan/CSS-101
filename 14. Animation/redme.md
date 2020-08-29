# Transition

    using this property you can amke the property change obsorvable.
    transformation porperties are all wachable example opacity,translate to these properties delay can be added so that transformation can be obsorved

    transition takes upto 4 comma seprated values
    each value is combination of poepertie name that you want to obsorve the change and delay 

    Example below when open class is addedd to div then the opacity change is prolonged to 500ms and you can obsorve the change from 0 to 1
```css
div{
    opacity:0;
    transition;opacity 500ms;
}

.open{
    opacity:1;
}
```

#  animate

    this feature of css allows creation of custom animation and apply to element.
    By doing element's size,shape,color.. can be changed and make it play in loop

    to create custom animation first animation needs to be defined

### keyframe

    animation frames can be defined by using @keyframe decorator, followed by the name of animation it can be any name you want

    it has mainly 2 sub feature

    from and to 

    from: inside this inital propertie for element can be defined 

    to: inside this final propertie that element should be transformed to will be defined

```css
@keyframe customname{
    from{
        transform:rotateZ(10deg);
    }
    to{
        transform:rotateZ(20deg);
    }
}
```
    in the above example if customname is applied to any element it will take inital position of 10 deg and further rotate it by 20deg

    to hove more frames in animation defined using keyframe it can take the proepertie as % that defiens the animmation completion percentage

```css
@keyframe customname2{
    0%{
        ransform:rotateZ(0deg);
    }
    50%{
        transform:rotateZ(10deg);
    }
    100%{
        transform:rotateZ(10deg);
    }
}
```

### animation
    to apply to element we use the property animation on element

    it is space seprated field with takes the following values

    first value:  name of the keyframe
    second value: how many milli seconds it should play
    third value: how much delay it should take before statring to play
    forth value: how many times it should repeat
    fifth value: after end of the animation before starting next frame what postion should be element in valid prperties are alternate,alternate-reverse,reverse

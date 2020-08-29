# Transition

using this property you can make the property change observable.
transformation properties are all watchable example opacity, translate to these properties delay can be added so that transformation can be observed

the transition takes upto 4 commas separated values
each value is a combination of properties name that you want to observe the change and delay 

The example below when open class is added to div then the opacity change is prolonged to 500ms and you can observe the change from 0 to 1

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

this feature of css allows the creation of custom animation and apply to the element.
By doing an element's size,shape,color.. can be changed and make it play in loop

to create custom animation first animation needs to be defined

### keyframe

animation frames can be defined by using @keyframe decorator, followed by the name of animation it can be any name you want

it has mainly 2 sub feature

from and to 

from: inside this initial properties for element can be defined 

to: inside this final properties that element should be transformed to will be defined

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
in the above example if customname is applied to any element it will take initial position of 10 deg and further rotate it by 20deg

to hove more frames in animation defined using keyframe it can take the property as % that defines the animation completion percentage

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
to apply to element we use the property animation on an element

it is space separated field with takes the following values

first value:  name of the keyframe
second value: how many milliseconds it should play
third value: how much delay it should take before starting to play
forth value: how many times it should repeat
fifth value: after end of the animation before starting next frame what position should be an element. valid properties are alternate,alternate-reverse,reverse

```css
div{
    animation:customname 200ms 10ms 4 alternate;
}

```
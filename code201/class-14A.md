# CSS Transforms, Transitions, and Animations

## Transforms: 
Transform Property this make a transformation to an element and allow us to to rotate, scale, move, and skew, HTML elements.

Transform Property comes in two different settings, 2D and 3D.

Transform Syntax#transform-syntax:`transform: scale(1.5);`

### 2D Transforms
2d transforms work on the x and y axes.

#### 2D Properties :
* 2D Rotate: We can use it to rotate an element form 0 to 360 degrees.
* 2D Scale: we can use it to change the size of an element.
* 2D Translate: We can use it to change the position of an element.
* 2D Skew: we can use it to  to distort an element.
* We can combining transforms to use multiple transforms at once ex:`transform: skew(10deg, 20deg) translateX(20px);`
* Transform Origin: we can use it to change the default transform.
* Perspective: we use it to work 3d transforms for an element.

### 3D Transforms:
2d transforms work on the x , y , z axes.

#### 2D Properties :
* 3D Rotate: We can use it to rotate an element in the three dimensions.
* 3D Scale : We can use it to Scale on the z axis.
* 3D Translate: We can use it it to change the position on the z axis.
* Backface Visibility: we set it's property to hidden, and it will hide the element whenever it is facing away from the screen.

***

## Transitions: 
Transitions Property allows us to change property values smoothly, over a given duration.

to use it we must specify the css property and the the duration of the effect.

### Transitions Property:
We use it to select  properties that we want to change.

#### Some of Transitions properties :
* background-color
* border-width
* clip
* font-size
* padding
* etc ..

### Transition Duration:
 We can use it to control the timming of the Transition.

Timing values:
* seconds 
* milliseconds 

### Transition Timing:
We can use transition-timing-function property  to set the speed in which a transition will move.

Transition-timing values:
* linear
* ease-in
* ease-out  
* ease-in-out
### Transition Delay;
we can use it  determines how long a transition should be stalled before executing.

***

## Animations
We use animations to change an element style to another specific style.

### Animations Keyframes
We use it To set multiple points of times for how the element change it style.

Keyframes rules:
* Animation name
* animation breakpoints
* properties to be animated

To use animation we must use :
1. Animation Name ex:`animation-name: slide;`
2. Animation Duration ex:`animation-duration: 4s;`
3. Timing Function ex:`  animation-timing-function: ease-in-out;`
4. Delay ex `animation-delay: .5s;`

### Animation Iteration
We can use it to make the animation repeat itself.
ex:`animation-iteration-count: infinite;`

### Animation Direction
We use it the set the directions of the Animation

Animation Direction values:
* normal
* reverse
* alternate
* alternate-reverse.

### Animation Play State
We use it allows an animation to be played or paused using the running and paused keyword values respectively.
 
ex:`animation-play-state: paused;`

### Animation Fill Mode
We can use it to identifies how an element should be styled either before, after, or before and after an animation is run.

Animation Fill Mode values:
* none
* forwards
* backwards
* both
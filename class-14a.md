# Transforms

With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the **transform property**.

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

### Transform Syntax

The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

![](https://www.w3.org/TR/css-transforms-1/examples/translate1.svg)

### 2D Transforms

Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes.


Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth.

**2D Rotate**

The rotate value provides the ability to rotate an element from 0 to 360 degrees. 

Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. 

The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically. 

**2D Scale**

Using the scale value within the transform property allows you to change the appeared size of an element. 

The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.

The scaleX value will scale the width of an element while the scaleY value will scale the height of an element.

To scale both the height and width of an element but at different sizes, the x and y axis values may be set simultaneously. 

To do so, use the scale transform declaring the x axis value first, followed by a comma, and then the y axis value.

**2D Translate**

The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. 

Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.

As with the scale value, to set both the x and y axis values at once, use the translate value and declare the x axis value first, followed by a comma, and then the y axis value.

The distance values used within the translate value may be any general length measurement, most commonly pixels or percentages. 

Positive values will push an element down and to the right of its default position while negative values will pull an element up and to the left of its default position.

**2D Skew**

The last transform value in the group, skew, is used to distort elements on the horizontal axis, vertical axis, or both.

The syntax is very similar to that of the scale and translate values. Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis. 

To distort an element on both axes the skew value is used, declaring the x axis value first, followed by a comma, and then the y axis value.%p

The distance calculation of the skew value is measured in units of degrees. Length measurements, such as pixels or percentages, do not apply here.

**Combining Transforms**

It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example. In this event multiple transforms can be combined together. To combine transforms, list the transform values within the transform property one after the other without the use of commas.

Using multiple transform declarations will not work, as each declaration will overwrite the one above it. The behavior in that case would be the same as if we were to set the height of an element numerous times.

**Transform Origin**

The transform-origin property can accept one or two values. When only one value is specified, that value is used for both the horizontal and vertical axes. If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis.

**Perspective**

The perspective for each element can be thought of as a vanishing point, similar to that which can be seen in three-dimensional drawings.

* Perspective Depth Value
* Perspective Origin

### 3D Transforms

* 3D Rotate: use three new transform values, including rotateX, rotateY, and rotateZ.
* 3D Scale:  the scaleZ three-dimensional transform elements may be scaled on the z axis.
* 3D Translate: Elements may also be translated on the z axis using the translateZ value. A negative value here will push an element further away on the z axis, resulting in a smaller element. Using a positive value will pull an element closer on the z axis, resulting in a larger element.
* 3D Skew: Skew is the one two-dimensional transform that cannot be transformed on a three-dimensional scale.
* Shorthand 3D Transforms

**Transform Style**

The transform-style property needs to be placed on the parent element, above any nested transforms. 

The preserve-3d value allows the transformed children elements to appear in their own three-dimensional plane while the flat value forces the transformed children elements to lie flat on the two-dimensional plane.

## Transitions & Animations

One evolution with CSS3 was the ability to write behaviors for transitions and animations

With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

There are four transition related properties in total, including:

* transition-property
* transition-duration
* transition-timing-function
* transition-delay

The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties.

Transitional Properties:

* background-color
* background-position
* border-color
* border-width
* border-spacing
* bottom
* clip
* color
* crop
* font-size
* font-weight
* height
* left
* letter-spacing
* line-height
* margin
* max-height
* max-width
* min-height
* min-width
* opacity
* outline-color
* outline-off
* setout
* line-width
* padding
* right
* text-indent
* text-shadow
* top
* vertical-align
* visibility
* width
* word-spacing


the background property is the only property that will change over the duration of 1 second in a linear fashion.

**Transition Duration**

The duration in which a transition takes place is set using the transition-duration property. 

The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms).

**Transition Timing**

The transition-timing-function property is used to set the speed in which a transition will move. Knowing the duration from the transition-duration property a transition can have multiple speeds within a single duration.

**Transition Delay**

On top of declaring the transition property, duration, and timing function, you can also set a delay with the transition-delay property.


**Animations** within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

**Animations Keyframes**

To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

**Animation Name**

Once the keyframes for an animation have been declared they need to be assigned to an element. To do so, the animation-name property is used with the animation name, identified from the @keyframes rule, as the property value. The animation-name declaration is applied to the element in which the animation is to be applied to.

**Animation Duration Timing Function, & Delay**

Once we have declared the animation-name property on an element, animations behave similarly to transitions. They include a duration, timing function, and delay if desired. To start, animations need a duration declared using the animation-duration property. As with transitions, the duration may be set in seconds or milliseconds.

**Animation Iteration**

By default, animations run their cycle once from beginning to end and then stop. To have an animation repeat itself numerous times the animation-iteration-count property may be used.

**Animation Direction**

On top of being able to set the number of times an animation repeats, we may also declare the direction an animation completes using the animation-direction property.

 Values for the animation-direction property include normal, reverse, alternate, and alternate-reverse.

**Animation Play State**

The animation-play-state property allows an animation to be played or paused using the running and paused keyword values respectively. 

When we play a paused animation, it will resume running from its current state rather than starting from the very beginning again.

**Animation Fill Mode**

The animation-fill-mode property identifies how an element should be styled either before, after, or before and after an animation is run. 

The animation-fill-mode property accepts four keyword values, including none, forwards, backwards, and both.

### CSS3 TRANSITIONS


CSS3 has introduced countless possibilities for UX designers, and the best thing about them is that the coolest parts are really simple to implement.

The transition property has three values: 
* the properties to transition 
* the speed of the transition
* third value which lets us change how the acceleration and deceleration is calculated

**Fade in**

Fade in effects are coded in two steps: first, we set the initial state; next, we set the change, for example on hover:

**Change color**

set the div’s class to “color” and specify the color we want in our CSS.

**Grow & Shrink**

To grow an element, we used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.

**Rotate elements**

CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element. 

**Square to circle**

A really popular effect at the moment is transitioning a square element into a round one, and vice versa. With CSS, it’s a simple effect to achieve, we just transition the border-radius property.

**3D shadow**

3D shadows were frowned upon for a year or so, because they weren’t seen as compatible with flat design, which is of course nonsense, they work fantastically well to give a user feedback on their interactions and work with flat, or fake 3D interfaces.

**Swing**

Not all elements use the transition property. We can also create highly complex animations using @keyframes, animation and animation-iteration.

**Inset border**

One of the hottest button styles right now is the ghost button; a button with no background and a heavy border. We can of course add a border to an element simply, but that will change the element’s position. We could fix that problem using box sizing, but a far simpler solution is the transition in a border using an inset box shadow.

![](https://engineerbabu.com/blog/wp-content/uploads/2019/01/CSS-Animation-Featured.jpg)


**6 Buttons animated**

    <div class="group">

		<button class="blam">Blam</button>

		<button style="-webkit-animation-delay: .3s;animation-delay: .3s;" class="syke">Syke</button>

		<button style="-webkit-animation-delay: .6s;animation-delay: .6s;" class="later">Later</button>

	</div>

**CSS3 Animations: Keyframes**

    @import url(https://fonts.googleapis.com/css?family=Montserrat:700);
    body {
     background-color: #ffcc46;
     }

     ::-webkit-scrollbar {
    width: 8px;
    }

     ::-webkit-scrollbar-thumb {
    background: rgba(0,0,0,0.12);
    }

    ::-webkit-scrollbar-track {
    visibility: hidden;
     }

     h1 {
     font-family: 'Montserrat', helvetica, arial;
    sans-serif;
    margin: 20px;
    }

    .exampleDiv {
    height: 200px;
    width: 200px;
    border: 1px solid rgba(0, 0, 0, 0.1);
    float: left;
    margin: 20px;
    text-align: center;
    position: relative;
    background-color: #ffffff;
     border-radius: 4px;
    }

    .ball {
     position: absolute;
    height: 20px;
    width: 20px;
    border-radius: 10px;
    background-color: #c0392b;
    }

    @-webkit-keyframes bouncing {
    40%, 70%, 90% {
    bottom: 0;
    -webkit-animation-timing-function: ease-out;
    }
     0% {
      bottom: 200px;
     left: 0;
    -webkit-animation-timing-function: ease-in;
     }
      55% {
    bottom: 50px;
      -webkit-animation-timing-function: ease-in;
    }
    80% {
    bottom: 25px;
      -webkit-animation-timing-function: ease-in;
    }
    95% {
    bottom: 10px;
    -webkit-animation-timing-function: ease-out;
     }
     100% {
    left: 110px;
    bottom: 0;
    -webkit-animation-timing-function: ease-out;
     }
       @-moz-keyframes bouncing {
      40%, 70%, 90% {
      bottom: 0;
      -webkit-animation-timing-function: ease-out;
       }
       0% {
      bottom: 200px;
      left: 0;
      -webkit-animation-timing-function: ease-in;
    }
    55% {
      bottom: 50px;
      -webkit-animation-timing-function: ease-in;
    }
    80% {
      bottom: 25px;
      -webkit-animation-timing-function: ease-in;
    }
    95% {
      bottom: 10px;
      -webkit-animation-timing-function: ease-out;
    }
    100% {
      left: 110px;
      bottom: 0;
      -webkit-animation-timing-function: ease-out;
    }

**404**

     body {
    margin:0;
     font-family:sans-serif;
    color:#f25252;
     background:#f7f7f7;
    }
    h1 {
    font-size:11rem;
    position:absolute;
    transform:translate(-50%,-50%);
    margin:0;
    }
    h1:nth-of-type(1){
    animation: range 4s infinite;
    }
    h1:nth-of-type(2){
    left:50%;
    top:50%;
     animation: size 4s infinite;
    }
    h1:nth-of-type(3){
    animation: range2 4s infinite;
    }
    @keyframes range {
    0%  {left:42%;top:50%;font-size:11rem;}
    25% {left:50%;top:40%;font-size:4.5rem;}
    50% {left:58%;top:50%;font-size:11rem;}
    75% {left:50%;top:60%;font-size:4.5rem;}
    100%{left:42%;top:50%;font-size:11rem;}
    }
     @keyframes range2 {
    0%  {left:58%;top:50%;font-size:11rem;}
     25% {left:50%;top:60%;font-size:4.5rem;}
     50% {left:42%;top:50%;font-size:11rem;}
    75% {left:50%;top:40%;font-size:4.5rem;}
     100%{left:58%;top:50%;font-size:11rem;}
    }
    @keyframes size {
     0%  {font-size:11rem;}
     25% {font-size:26rem;}
     50% {font-size:11rem;}
    75% {font-size:26rem;}
     100%{font-size:11rem;}
    }

**Pure CSS Bounce Animation**

	   <div class="animation animation-1">
		<div class="ball"></div>
     	</div>
    	<div class="animation animation-2">
		<div class="ball"></div>
       </div>
     	<div class="animation animation-3">
		<div class="ball"></div>
	   </div>	
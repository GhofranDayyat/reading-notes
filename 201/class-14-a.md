# What Google Learned From Its Quest to Build the Perfect Team
 ## Good teams Specifications:
*  what distinguished the ‘‘good’’ teams from the dysfunctional groups was how teammates treated one another. 
*  could raise a group’s collective intelligence, whereas the wrong norms could hobble a team, even if, individually, all the members were exceptionally bright.
* Equality in distribution of conversational turn-taking
* average social sensitivity toward their colleagues

### Psychological safety is ‘‘a sense of confidence that the team will not embarrass, reject or punish someone for speaking up

# CSS Transforms
**categorized into** 
1. 2D Transforms (Two-dimensional transforms) :works in x-axis and y-axis.
2. 3D Transforms (Three-dimensional transforms):works in x-axis ,y-axis and z-axis.

## 2D Rotate 
* ability to rotate an element from 0 to 360 degrees
*  a positive value will rotate an element clockwise``transform: rotate(20deg);``

*  a negative value will rotate the element counterclockwise``transform: rotate(-55deg);``

## 2D Scale
* Using the scale value within the transform property allows you to change the appeared size of an element. 
* The default scale value is 1
*  any value between .99 and .01 makes an element appear smaller``transform: scale(.75);``
* any value greater than or equal to 1.01 makes an element appear larger``  transform: scale(1.25);``
* scaleX value will scale the width of an element while the scaleY value will scale the height of an element. 
``  transform: scaleX(.5);``  ``  transform: scaleY(1.15);``
* scale both the height and width of an element but at different sizes**x axis value first**
  ``transform: scale(.5, 1.15);``

## 2D Translate
* The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document.
*  translateX value will change the position of an element on the horizontal axis``transform: translateX(-10px);``

* translateY value will change the position of an element on the vertical axis.``transform: translateY(25%);``
*  set both the x and y axis values at once ``transform: translate(-10px, 25%);``

## 2D Skew
* horizontal axis``transform: skewX(5deg);``
* vertical axis ``transform: skewY(-20deg);``
* both``transform: skew(5deg, -20deg);``

## Combining Transforms
It is common for multiple transforms to be used at once
`` transform: skew(10deg, 20deg) translateX(20px);``

`` transform: rotate(25deg) scale(.75);``


# Transitions & Animations

The easiest way for determining styles for different states is by using the *:hover, :focus, :active, and :target* **pseudo-classes.**

**Transitions**: 
1. transition-property
2. transition-duration
3. transition-timing-function
4.  transition-delay

``.box:hover {``

 `` background: #ff7b29;``

``}``
*  properties identified within the transition-property value will be affected by any transitions.
* all of the properties within an element’s different states will be altered upon change

## Vendor Prefixes
 For the best support across all browsers, use vendor prefixes.
 ``-webkit-transition-property: background;``
 ``-moz-transition-duration: 1s;``
 ``-o-transition-timing-function: linear;``

## Transitional Button
button {``transition: all .1s linear;``}

``button:active {``

  ``box-shadow: 0 2px 0 #006599;``

  ``transform: translateY(3px);``
``}``


# Animations
do a great job of building out visual interactions

* **Animations Keyframes** includes the*animation name*, any *animation breakpoints*, and the *properties intended* to be animated.

* Vendor Prefixing the Keyframe Rule
1. @-moz-keyframes
2. @-o-keyframes
3. @-webkit-keyframes

* Animation Name
``animation-name: slide;``

* Animation Duration, Timing Function, & Delay
``animation-duration: 2s;``
``animation-timing-function: ease-in-out;``
``animation-delay: .5s;``

* Animation Iteration
``animation-iteration-count: infinite;``

* Animation Direction
``animation-direction: alternate;``

* Animation Play State
``animation-play-state: paused;``


# 8 really simple effects in css

1. Fade in
``.fade``

``{``
        ``opacity:0.5;``

``}``

``.fade:hover``

``{``

``opacity:1;``

``}``

2. Change color

``.color:hover``

``{``

 `` background:#53a7ea;``

``}``

3. Grow & Shrink
``.grow:hover``

``{``

``-webkit-transform: scale(1.3);``

``-ms-transform: scale(1.3);``

``transform: scale(1.3);``
``}``

``.shrink:hover``
``{``

 ``-webkit-transform: scale(0.8);``

``-ms-transform: scale(0.8);``

 ``transform: scale(0.8);``
``}``


4. Rotate elements
``.rotate:hover``
``{``

 `` -webkit-transform: rotateZ(-30deg);``

 ``  -ms-transform: rotateZ(-30deg);``

  ``  transform: rotateZ(-30deg);``
``}``

5. Square to circle
``.circle:hover``

``{``

`` border-radius:50%;``
``}``

6. 3D shadow
``.threed:hover``

``{``

``box-shadow:``

``1px 1px #53a7ea,``

 `` 2px 2px #53a7ea,``

 `` 3px 3px #53a7ea;``

``-webkit-transform: translateX(-3px);``

 ``` transform: translateX(-3px);```

``}``

7. Swing
``.swing:hover``

``{``

 ``       -webkit-animation: swing 1s ease;``

 ``       animation: swing 1s ease;``

``       -webkit-animation-iteration-count: 1;``

``        animation-iteration-count: 1;``

``}``


8. Inset border
``.border:hover``

``{``

  ``      box-shadow: inset 0 0 0 25px #53a7ea;``
  
``}``




















